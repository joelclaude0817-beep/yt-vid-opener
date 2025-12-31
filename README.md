# 🎬 YouTube Video Opener for Termux

A simple and elegant Python script that allows you to search and open YouTube videos directly from your Termux terminal with a beautiful interface!

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Termux-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## ✨ Features

- 🔍 Search YouTube videos from terminal
- 🎯 Open direct YouTube video URLs
- 🎨 Beautiful terminal interface with banner
- ⚡ Animated "Opening..." message
- 📱 Opens videos in YouTube app or browser
- ❌ Helpful error messages and setup instructions

## 📋 Prerequisites

Before using this script, you need to have:

- **Termux** installed on your Android device
- **Python 3.x**
- **Termux-API** package

## 🚀 Installation

### Step 1: Install Required Packages

Open Termux and run:

```bash
pkg update && pkg upgrade
pkg install python termux-api
```

### Step 2: Install Termux:API App

Download and install the **Termux:API** app from the same source where you got Termux:
- [F-Droid](https://f-droid.org/packages/com.termux.api/)
- [GitHub Releases](https://github.com/termux/termux-api/releases)

⚠️ **Important:** Both Termux and Termux:API must be from the same source (both from F-Droid or both from GitHub).

### Step 3: Download the Script

```bash
# Clone this repository
git clone https://github.com/joelclaude0817-beep/youtube-video-opener.git
cd youtube-video-opener

# Or download directly
curl -O https://raw.githubusercontent.com/joelclaude0817-beep/youtube-video-opener/main/yt_opener.py
```

### Step 4: Make Script Executable

```bash
chmod +x yt_opener.py
```

## 📖 Usage

### Basic Usage

**Search for videos:**
```bash
python yt_opener.py python tutorial
```

**Open a direct YouTube URL:**
```bash
python yt_opener.py https://youtube.com/watch?v=dQw4w9WgXcQ
```

### Create an Alias (Optional but Recommended)

For easier access, add an alias to your `.bashrc`:

```bash
echo 'alias yt="python ~/youtube-video-opener/yt_opener.py"' >> ~/.bashrc
source ~/.bashrc
```

Now you can simply use:
```bash
yt python tutorial
yt https://youtube.com/watch?v=VIDEO_ID
```

## 🎯 Examples

```bash
# Search for tutorials
python yt_opener.py termux tutorials

# Search for music
python yt_opener.py lofi hip hop

# Open a specific video
python yt_opener.py https://www.youtube.com/watch?v=dQw4w9WgXcQ

# Multi-word searches
python yt_opener.py how to code in python
```

## 🖥️ Screenshot Example

```
╔═══════════════════════════════════════╗
║     YouTube Video Opener v1.0         ║
╚═══════════════════════════════════════╝

🎬 Opening [python tutorial]... ✓

✅ Video opened successfully!
```

## 🔧 Troubleshooting

### Error: "termux-open-url not found"

**Solution:** Install the termux-api package:
```bash
pkg install termux-api
```

Also ensure you have the Termux:API app installed from the same source as your Termux app.

### Video doesn't open

**Possible causes:**
1. No internet connection
2. Termux:API app not installed
3. Permissions not granted to Termux:API

**Solution:** Grant all permissions to Termux:API in Android settings.

### Script shows "Permission denied"

**Solution:** Make the script executable:
```bash
chmod +x yt_opener.py
```

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 💡 Future Enhancements

Ideas for future versions:
- Video history tracking
- Favorite searches
- Download video options
- Playlist support
- Video quality selection
- Search suggestions

## 👏 Acknowledgments

- Built for the Termux community
- Inspired by the need for quick YouTube access from terminal
- Thanks to all contributors

## 📧 Contact

If you have any questions or suggestions, feel free to:
- Open an issue on GitHub
- Submit a pull request
- Contact the maintainer

---

**Made with ❤️ for Termux users**

⭐ If you find this useful, please star the repository!
