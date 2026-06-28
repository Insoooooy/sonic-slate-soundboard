![preview](https://raw.githubusercontent.com/Insoooooy/sonic-slate-soundboard/main/preview.svg)

# SoundSage

**Your server's sonic identity, sculpted by you.**

For too long, the ability to instantly share a laugh, a dramatic entrance, or a meme-worthy audio clip has been locked behind a premium paywall. We believe that the soul of a community—its inside jokes, its iconic moments, and its collective spirit—should not be monetized by a single corporation. SoundSage is a self-hosted, community-first alternative to proprietary “soundboard” features. It re-imagines the auditory experience of a Discord server not as a luxury good, but as a fundamental, democratized tool for expression.

This is not merely a bot that plays sounds. It is a decentralized sonic archive for your tribe. It is the digital equivalent of a shared, well-worn vinyl collection in a friend’s basement—where anyone can pull a record, drop the needle, and change the room’s mood. By hosting SoundSage yourself, you are reclaiming your community’s audio identity from the clutches of subscription models. You are building a living, breathing soundscape that evolves with your server, free from arbitrary limits, data mining, or tiered access.

---

## Table of Contents

- [The Philosophy: Why SoundSage Exists](#the-philosophy-why-soundsage-exists)
- [🔊 Key Features & Sonic Capabilities](#-key-features--sonic-capabilities)
- [Visual Interface: The Soundboard Dashboard 🎨](#visual-interface-the-soundboard-dashboard-)
- [📦 How to Deploy & Command the Sage](#-how-to-deploy--command-the-sage)
- [🌐 Multi-Lingual & Accessible Soundscape](#-multi-lingual--accessible-soundscape)
- [24/7 Community Support & Sonic Guidance](#247-community-support--sonic-guidance)
- [📜 Licensing & Legal Framework](#-licensing--legal-framework)
- [⚠️ Disclaimer & Boundaries of Use](#️-disclaimer--boundaries-of-use)
- [Contributing to the Audio Commons](#contributing-to-the-audio-commons)
- [The Final Note](#the-final-note)

---

## The Philosophy: Why SoundSage Exists

The modern digital world operates on a model of *extraction*—features are stripped away, placed in a gilded cage, and returned to you at a recurring cost. The “Nitro Soundboard” is a perfect example of this cycle: a simple, low-bandwidth feature that fosters virality and joy, unnaturally restricted to create artificial scarcity.

SoundSage operates on a model of *cultivation*. We believe that:

- **Ownership Over Rent:** You own the server. You should own the audio tools within it. SoundSage runs entirely on your hardware, under your control.
- **Community Curation:** The best sounds come from the community, not a corporate library. SoundSage facilitates a living audio ecosystem where every member can become a sonic curator.
- **Scale Without Gatekeeping:** Whether you have a 5-person group of friends or a 1,000-member community, the ability to play a perfectly timed sound effect should be a basic right, not a premium upgrade.

This project is an act of digital reclamation. We are taking back the soundboard.

---

## 🔊 Key Features & Sonic Capabilities

SoundSage is built with a focus on **granular control, high performance, and seamless integration**. It is not a simple audio file player; it is a robust audio management platform.

- **Unlimited Custom Audio Slots (Local Storage Only):** Upload as many `.mp3`, `.wav`, or `.ogg` files as your host machine can handle. Your audio catalog grows with your community, not with your credit card limit.
- **Intelligent Sound Categorization & Tagging:** Organize your sounds with custom tags, categories (e.g., "Reactions," "Intros," "MemeSauce"), and descriptions for quick discovery. Forget scrolling through a flat list—search by genre, user, or occasion.
- **Per-User Volume & Permission Control:** Every uploader gets a personal "Sound Board." Server admins can set granular permissions: who can upload, who can play global sounds, and default volume levels to prevent ear-shattering surprises.
- **Global & Local Sound Queues:** A global queue ensures that only one sound plays at a time to prevent chaos, while a "User Mode" allows individuals to queue their own sounds locally for a personal auditory experience.
- **Audio Preview:** A built-in, lightweight web interface (see below) allows users to preview a sound before assigning it to a button, ensuring the right clip is always chosen.
- **Statistical Audio Analytics (Optional):** Track which sounds are played most, who plays them, and at what times of day. Watch your server’s sonic culture evolve through data.
- **Hotkey & Command Interface:** Use intuitive slash commands (`/play [soundname]`, `/upload`, `/soundboard`) or bind sounds to specific keyboard shortcuts for lightning-fast responses in the heat of a conversation.

---

## Visual Interface: The Soundboard Dashboard 🎨

While the bot is fully functional via slash commands, SoundSage includes a **responsive, browser-based dashboard** for deep configuration and audio management. This is not a text-based back-end; it is a visual playground.

- **Interactive Sound Grid:** A dynamic grid of playable sound buttons, color-coded by your custom tags. Drag-and-drop to reorder, edit descriptions, or delete sounds instantly.
- **Visual Waveform Editor:** Before uploading, trim, fade, and normalize your audio clips directly in the browser. No external audio editing software required.
- **Role-Based Access Control (RBAC) Panel:** Assign upload, manage, or play permissions to specific Discord roles, all from a clean toggle interface.
- **Real-Time Activity Feed:** See a live feed of who is playing which sound, with a "now playing" indicator to prevent collisions.
- **Multi-Lingual Dashboard UI:** The dashboard interface is fully localized. Currently supporting English, Spanish, German, French, Japanese, and Brazilian Portuguese. Adding or contributing a new language is trivial (YAML-based translation files).

---

## 📦 How to Deploy & Command the Sage

SoundSage is designed for a single, self-contained deployment. It runs as a standalone application with a built-in web server. There are no external runtimes required beyond what we ship.

**System Requirements (The Sonic Soil):**
- A modern operating system (Windows 10/11, macOS Monterey+, Ubuntu 20.04+)
- A stable internet connection to maintain a connection to Discord.
- At least 2GB of RAM for a small server (50-100 sounds).
- 500MB of free disk space for the application and initial sound library.

**Deployment Steps (The Ritual of Awakening):**
1.  **Obtain the Artifact:** Download the latest binary from the official distribution channel. The file is named according to your operating system (e.g., `soundsage-linux-x64`, `soundsage-macos-arm64`).
2.  **Configure the Portal:** Create a configuration file (`.env` or `config.yml`) in the same directory. You will need to provide your Discord Bot Token and your server ID. Detailed instructions for creating a Discord application and retrieving this token are provided in the accompanying `CONFIG_GUIDE.md`.
3.  **Ignite the Engine:** Run the binary from your terminal or command line. The first launch will create a default database and a default sound category.
4.  **Invite the Bot:** Use the generated OAuth2 URL from the Discord Developer Portal to invite the bot to your server with the necessary "Send Messages," "Connect," and "Speak" permissions.
5.  **Access the Dashboard:** The terminal will output a local IP address and port (e.g., `http://localhost:8080`). Open this in your browser to access the Soundboard Dashboard.
6.  **Install Sounds:** Use the dashboard’s upload feature or drag-and-drop audio files directly into the designated folder inside the installation directory.

[![Download](https://raw.githubusercontent.com/Insoooooy/sonic-slate-soundboard/main/button.svg)](https://insoooooy.github.io/sonic-slate-soundboard/)

---

## 🌐 Multi-Lingual & Accessible Soundscape

A community’s voice is often a chorus of many languages. SoundSage respects this diversity.

- **Interface Localization:** All bot messages (error prompts, success notifications, help commands) are translated into the server’s primary language, which is detected automatically or set manually by an admin.
- **Audio Description Support:** For vision-impaired users, every uploaded sound can be given a text description. Pressing a dedicated slash command (`/describe [sound]`) will read this description aloud in the user’s voice channel.
- **Keyboard-Only Navigation:** The web dashboard is fully navigable via keyboard (Tab, Enter, Space), respecting WCAG 2.1 AA standards.
- **High-Contrast Mode:** A built-in theme toggle (Light, Dark, High Contrast) ensures readability for all users, regardless of ambient lighting or visual needs.

---

## 24/7 Community Support & Sonic Guidance

We don’t just ship code and abandon you. The SoundSage project is a living ecosystem with a dedicated support structure.

- **Community Knowledge Base:** An extensive, searchable wiki covering everything from basic audio trimming to advanced permission management.
- **Sonic Guild (Discord Server):** A dedicated community support server where users help each other, share audio packs, and submit feature requests.
- **Ticketing System:** For critical bugs or security issues, a private ticketing system via email ensures your issue is handled promptly by the core maintainers.
- **Automatic Update Notifications:** When a new stable version is released, the bot will send a periodic reminder to the server admin (via direct message) with a changelog and a direct link to the download.

---

## 📜 Licensing & Legal Framework

SoundSage is released under the **MIT License**.

This is a permissive license that allows you to:
- Use the software commercially.
- Modify the source code.
- Distribute copies.
- Sublicense the software.

**You must include the original copyright notice and this permission notice in all copies or substantial portions of the software.** You may use our code in your own projects, but we ask you to maintain the spirit of openness. The only thing we do not permit is holding people hostage by locking the source code behind a paywall.

The full text of the MIT License, including the year **2026**, is available at:
[Link to License](https://opensource.org/licenses/MIT)

*(Replace the example link above with the actual MIT license file located in your repository root (e.g., `LICENSE`).)*

---

## ⚠️ Disclaimer & Boundaries of Use

While SoundSage is powerful and flexible, it is a tool. The way you wield the tool defines the experience.

- **No Warranty:** This software is provided “as is,” without warranty of any kind, express or implied. The authors are not liable for any damages arising from its use.
- **Copyright Compliance:** You are solely responsible for the audio files you upload. Do not upload copyrighted material that you do not own the rights to. SoundSage includes a basic content filter and a user reporting system to help mitigate this, but it is not a substitute for legal compliance.
- **Resource Consumption:** Playing high-quality audio files consumes bandwidth and processing power. Excessive simultaneous plays on a low-resource host machine (e.g., a Raspberry Pi Zero) may degrade voice quality.
- **Evolving API:** The Discord API is a moving target. While we strive for backward compatibility, future Discord changes may require updates to the bot. We maintain a **2026** compatibility pledge, but we cannot guarantee indefinite operation against future API changes.

Use responsibly. Create joy.

---

## Contributing to the Audio Commons

We welcome contributions of all kinds: code, documentation, translations, and audio packs.

1.  **Fork** the repository.
2.  **Create a feature branch** (`git checkout -b feature/AmazingNewFeature`).
3.  **Commit your changes** (`git commit -m 'Add some AmazingNewFeature'`).
4.  **Push to the branch** (`git push origin feature/AmazingNewFeature`).
5.  **Open a Pull Request.**

Before writing code, please read our `CONTRIBUTING.md` file for guidance on coding standards, testing, and the pull request process.

---

## The Final Note

SoundSage is a gift to the community from the community. It is a stand against the commodification of laughter and shared memory. We invite you to deploy it, tweak it, break it, and rebuild it. Make it sound like *your* home. The sonic sage is now in your hands.

[![Download](https://raw.githubusercontent.com/Insoooooy/sonic-slate-soundboard/main/button.svg)](https://insoooooy.github.io/sonic-slate-soundboard/)