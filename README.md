Nova · Observatory Chat

A single-file, self-contained AI chat interface with a star-chart aesthetic — deep void backgrounds, a live constellation canvas, and warm starlight-gold accents. Talks to Groq's chat API and runs entirely in your browser.

Features


Multiple conversations — create, search, pin, and delete chats, all saved in your browser's local storage
Live constellation background — stars connect with faint lines when near each other or your cursor, with occasional shooting stars
Rich messages — markdown-style bold/italic/inline code, syntax-styled code blocks with a copy button, date separators ("Today" / "Yesterday"), copy / like / regenerate on any message
Customizable — editable display name, five accent color themes, export any conversation to a .txt file
Responsive — collapsible sidebar on mobile, keyboard focus states, respects reduced-motion preferences


Getting started


Open nova-ai-chat.html in any modern browser (Chrome, Safari, Firefox, Edge). No build step, no server required.
Click the gear icon (⚙️) to open Settings.
Paste in a Groq API key. Get a free one at console.groq.com/keys.
Start chatting.


Your API key is stored only in your own browser's local storage — it is never sent anywhere except directly to Groq's API when you send a message.

Choosing a model

Use the model picker in the top-right of the chat header to switch between:

ModelNotesLlama 3.3 · 70BBest general-purpose qualityMixtral · 8x7BFaster, good for longer contextGemma 2 · 9BLightest and fastest

Data & privacy

Everything Nova stores lives in localStorage in your browser, under these keys:


nova_chats — your conversations and messages
nova_api_key — your Groq API key
nova_user_name, nova_accent, nova_active — display preferences


Use Settings → Clear all conversations to wipe your chat history, or clear your browser's site data for this file to remove everything, including the API key.

Known limitations


Attach and voice-input buttons are placeholders for now — they don't yet do anything.
No streaming responses; replies appear once fully generated.
Local storage has a size ceiling (usually several MB), so extremely long-running chat histories could eventually hit browser limits.

Everything lives in one file: nova-ai-chat.html. Open it, use it, or copy it — no dependencies to install beyond the Google Fonts loaded via CDN link in the <head>.
