TOTO.Ai — raccoon personality edition

NEW PROJECT IN GITHUB CODESPACES
1. Extract this ZIP. Open the TOTO-browser folder.
2. Create a new GitHub repository. Upload index.html, app.js, server.js, package.json, and this README.txt directly into the repository root.
3. Code > Codespaces > Create codespace.
4. Run npm start in the terminal. No npm install needed.
5. Open forwarded port 3000 in the browser.
6. Select a small model and click Load AI. First load downloads model files and may take several minutes.
7. For friends, change port 3000 visibility to Public and share its HTTPS URL. Anyone with the URL can open it; this starter has no login system. Each visitor needs compatible hardware and downloads their own model. Keep the Codespace running. Hosting quotas are separate from AI usage; not unlimited free hosting.

IF UPDATING THE PREVIOUS BROWSER STARTER
Replace app.js with this edition's app.js, then reload the webpage. Start a new chat and click Load AI. The other code files can also be replaced together as a complete update. Never overwrite Monopoly.

PERSONALITY
Occasionally says 'Tupid raccoon' when correcting a real mistake and 'Good raccoon' when agreeing. Explains its reasoning rather than mechanically choosing a phrase. Drops teasing for sensitive topics and when asked. Model compliance is not guaranteed, especially with small models.

REQUIREMENTS AND PRIVACY
- No Ollama or paid API keys. Uses WebLLM 0.2.87 from esm.run and models from hosts configured in WebLLM metadata.
- Requires HTTPS (or localhost), WebGPU, enough graphics memory, storage, and internet for downloads. Model downloads may be hundreds of MB or several GB. Browser caching can be cleared or evicted.
- The server only serves web files. AI processing happens in the visitor's browser. Chat messages are not sent to this project's server or a paid AI provider. Third parties receive ordinary library/model download requests.
- Saved history stays in this browser profile's localStorage. New chat deletes it. Do not use a shared browser profile for private conversations.
- Last 12 messages are used for context, subject to model limits. Older context can be forgotten. Start a new chat on context errors.
- No live search, videos, file uploads, or cross-device memory. Plain-text replies. One generation at a time. Small models may be inaccurate and do not match frontier assistants.
- VRAM estimates are not guarantees of total memory use. Some browsers/devices cannot run this app.
- This starter is not audited or production-hardened. It has not been tested against your browser/GPU. No friend-specific access controls are included.

Documentation: https://webllm.mlc.ai/docs/user/get_started.html
