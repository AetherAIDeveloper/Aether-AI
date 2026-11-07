<div align="center">

<img src="icon.png" alt="Aether AI" width="128" height="128">

# Aether AI

**A fast, beautiful AI assistant for your desktop.**
Dark, minimal, and able to read almost anything you throw at it.

[![Download for Windows](https://img.shields.io/badge/Download-Windows-8b93ff?style=for-the-badge&logo=windows&logoColor=white)](YOUR-DOWNLOAD-LINK)
[![Version](https://img.shields.io/badge/Version-1.1.0-17171a?style=for-the-badge)](YOUR-DOWNLOAD-LINK)
[![License: MIT](https://img.shields.io/badge/License-MIT-17171a?style=for-the-badge)](LICENSE)

</div>

<br>

<!-- Add a screenshot: save it as docs/screenshot.png, then delete this comment -->
<!-- <p align="center"><img src="docs/screenshot.png" alt="Aether AI screenshot" width="860"></p> -->

## Download

**[Download Aether AI for Windows →](YOUR-DOWNLOAD-LINK)**

1. Click the link above and download **`Aether AI Setup 1.1.0.exe`** from the page that opens.
2. Run the file. Aether installs in a few seconds and adds a Start menu entry and desktop shortcut.
3. Open **Aether AI** and start chatting. No account and no setup.

> **Windows says "Windows protected your PC"?** That is normal for new apps that aren't signed with a paid certificate. Click **More info**, then **Run anyway**.

## Why you'll like it

| | |
|---|---|
| **Three models** | **Blyx 3.1** for instant answers, **Zylo 4.5** for everyday use, and **Qira 5.5** when you need it to take its time and think a problem through. Switch any time from the top bar. |
| **Attach almost anything** | Images, PDFs, Word documents, text and code, audio and even video. Drag, drop or paste straight into the window. |
| **Replies that stream in** | Watch answers appear live, stop them whenever you like, and regenerate with one click. |
| **Code that's easy to use** | Clean code blocks with a one-click Copy button. |
| **Your history, organized** | Chats are grouped by Today, Yesterday and earlier, with instant search. |
| **Your rules** | Set custom instructions once and they apply to every chat. |
| **A calm, modern look** | Pure dark design, smooth animations, and nothing in the way. |

## What Aether can read

| You attach | What Aether does |
|---|---|
| **Images** | Looks at the image and answers questions about it |
| **Video** | Studies frames from across the video and transcribes what's said |
| **Audio** | Transcribes it to text |
| **PDF and Word (.docx)** | Reads the text inside |
| **Text and code files** | Reads them in full |

Aether can't read other file types, such as zip files and programs, and it will tell you when that happens.

## Tips

- **Drag and drop** files anywhere in the window, or **paste** an image with `Ctrl+V`.
- `Enter` sends, `Shift+Enter` adds a new line, `Ctrl+N` starts a new chat.
- Pick **Blyx 3.1** for quick questions and **Qira 5.5** for hard ones.
- Use **Settings** to give Aether standing instructions, like "keep answers short".

## FAQ

**Is it free?**
Yes. Download it and use it.

**Where are my chats stored?**
On your own computer. Messages and attachments are sent over the internet to generate replies, so you need to be online to chat.

**Does it work on Mac or Linux?**
The ready-made download is for Windows. Mac and Linux users can build it from source in a couple of minutes (see below).

**How do I uninstall it?**
Windows **Settings → Apps → Installed apps → Aether AI → Uninstall**.

## Build from source

You'll need [Node.js](https://nodejs.org) (the LTS version).

```bash
git clone https://github.com/YOUR-USERNAME/aether-ai.git
cd aether-ai
npm install
npm start
```

Create an installer for your system:

```bash
npm run build
```

The result appears in the `dist` folder (`.exe` on Windows, `.dmg` on Mac, AppImage on Linux).

Copy `config.example.js` to `config.js` and add your API key before the first run. You can also rename the models and edit their descriptions there.

> **Electron won't start after `npm install`?** Newer versions of npm block its setup script. Run
> `npm install-scripts approve electron`, then `npm rebuild electron`, then `npm start`.

## Built with

[Electron](https://www.electronjs.org), plus plain HTML, CSS and JavaScript. No framework.

## License

MIT
