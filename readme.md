# Fireflies: Convert Spotify Playlists to Apple Music!

Fireflies is a web application that makes it easy to convert your Spotify playlists to Apple Music. No more worrying about losing your music during the switch—it’s a smooth, free transition!

---

## How It Works

### Step 1: Enter Your Details
1. **Add your email.**
2. **Provide your Spotify Playlist ID.**
   - To find this, get the share link for your playlist on Spotify.
   - Example: If your share link is `https://open.spotify.com/playlist/2QwR5DBHrJYjWgH1YIuCeu?si=v1FASDLjQAWmaDH8FrSbhw&pi=a-AFnbboMERL2m`, the Playlist ID is `2QwR5DBHrJYjWgH1YIuCeu`.

3. **Press Submit.**
   - Your results will appear in the "Show Results" toggle.

---

### Step 2: Add Apple Music Authentication Tokens
To convert the playlist, Fireflies requires Apple Music authentication tokens.

**Follow these steps to extract the tokens:**

<details>
  <summary><strong>Guide to Extract Apple Music Tokens</strong></summary>
  <div style="border: 1px solid #ccc; padding: 15px; background-color: #f9f9f9; border-radius: 5px;">
    <ol>
      <li>Login to Apple Music in a browser.</li>
      <li>Open Developer Tools:
        - On Windows, press <code>Ctrl + Shift + C</code>
        - On Mac, press <code>Cmd + Shift + C</code>
      </li>
      <li>Go to the <strong>Network</strong> tab and filter for <code>Fetch/XHR</code> requests.</li>
      <li>In the Apple Music interface, click on the <strong>Recently Added</strong> section in the sidebar.</li>
      <li>From the request headers, copy the following keys:
        <ul>
          <li><strong>Authorization</strong>: Copy the code following "Bearer" (do not include "Bearer" or the space).</li>
          <li><strong>Media-user-token</strong></li>
        </ul>
      </li>
    </ol>
    <img src="apple_tokens_image.png" alt="Apple Music Tokens Guide Image" style="max-width: 100%; border: 1px solid #ccc; border-radius: 5px; margin-top: 15px;">
  </div>
</details>

---

### Step 3: Start the Conversion
1. Enter the tokens.
2. Press **Submit** to start converting your playlist!

Fireflies will take care of the rest.

---

Happy listening!
