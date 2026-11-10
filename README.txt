TOTO.Ai — Raccoon workspace edition

UPDATE EXISTING PROJECT
Replace index.html, server.js, and package.json with these files. This edition puts all browser JavaScript inside index.html. Your old app.js is no longer used and can be deleted.
In Codespaces save the files, stop the running server with Ctrl+C, then run npm start. Open port 3000 in a regular HTTPS browser tab and refresh the page. Load the AI and click New chat to use fresh personality instructions.
No npm install, paid API key, or Ollama is needed. The AI model still downloads into the browser. WebGPU and sufficient memory are required.

FEATURES
- Raccoon-themed prompt for informational replies; playful correction only for lighthearted mistakes, not sensitive topics. Small models may not follow the prompt reliably.
- Chat, coding, writing, study, and reasoning modes.
- Saved preferences, recent conversation, and a manually managed to-do list in localStorage.
- Text reference file selector: supported extensions only, under 32 KB and 8,000 characters. Reference text is held in memory and added to subsequent questions until removed. Reference text is NOT automatically restored on reload or saved with the conversation. New chat clears it.
- Copy entire reply, copy fenced code blocks, download reply/code blocks, export conversation or tasks.
- The code download extension is guessed from the code fence language. Filenames are generic and may need renaming. Files are not executed or tested.
- Longer responses option and Ask TOTO to continue. Continuation may repeat content or forget context. It is not autonomous multi-step execution.

LIMITATIONS
No live web search or verified citations, no video/image generation, no email/calendar integration, no GitHub editing, no computer control. The task list is manually controlled; the model does not automatically add tasks. The app does not claim a small model matches a frontier assistant.
Only the last 8 messages (up to 6,000 characters each) are submitted, subject to model context limits. Prompt and reference text add to context size. If a context error occurs, remove the reference or start a new chat. Longer output can increase generation time and memory demand.
The first model download can take a long time. Model sizes and VRAM estimates come from WebLLM metadata and are not guarantees. Browser cache eviction may require redownloads. No Web Worker is used; device responsiveness can vary.

PRIVACY AND SHARING
Conversation, preferences and tasks are in this browser profile's localStorage, not a server database. Other people using that browser profile can see them. New chat does not clear tasks or preferences; delete tasks and erase/save preferences separately to clear those. Clearing browser site storage removes all local data and may remove cached models.
WebLLM 0.2.87 loads from esm.run, and model downloads use hosts in its configuration. This app does not send your chat messages or file text to an AI server. Third parties still receive ordinary resource download requests. This starter is not audited or production-hardened.
For friends, make Codespaces port 3000 public and share its HTTPS URL. Anyone with the link can open it; no login system included. Each visitor runs their own model. Website availability depends on hosting; Codespaces quotas and billing are separate from AI usage. Keep it within your free allowance if avoiding charges.

TESTING
Generated files have not been tested in your browser or against your GPU. Test loading and a short chat before using reference files or sharing.
Official docs: https://webllm.mlc.ai/docs/user/basic_usage.html
