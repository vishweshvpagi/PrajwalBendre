# 🎭 AR Flashcards - Meme Edition

An interactive **WebAR (Web-based Augmented Reality)** experience that brings popular meme characters to life in 3D. Just point your mobile camera at flashcard images and watch them appear as animated 3D models in real-time — no app required!

[![Live Demo](https://img.shields.io/badge/Demo-Live-success)](https://vishweshvpagi.github.io/PrajwalBendre/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

---

## 🚀 Live Demo
👉 **Try it now on your mobile device:**  
🔗 https://vishweshvpagi.github.io/PrajwalBendre/

---

## ✨ Features
- 📱 Browser-based Augmented Reality (no installation needed)
- 🎯 Multi-image target recognition
- 🌀 Animated 3D GLTF models using Three.js
- 🌐 Works on iOS and Android browsers
- ⚡ Fast loading via CDN
- 🔈 Audio-ready architecture

---

## 🎮 How to Use

### ✅ Method 1: View Online (Recommended)
1. Open the live link.
2. Allow camera access.
3. Point your camera at the flashcard images.
4. Watch the meme characters come alive!

### 💻 Method 2: Run Locally
```bash
git clone https://github.com/vishweshvpagi/PrajwalBendre.git
cd PrajwalBendre
```
Start a server:
```bash
# Using Python
python -m http.server 8000
# OR using Node
npx http-server -p 8000
```
Open `http://localhost:8000` in your browser and allow camera permissions.

---

## 📸 Flashcard Targets

| Image File     | Character  | Description            |
|----------------|------------|------------------------|
| tungutung.jpg  | Tung Tung  | Internet meme legend   |
| tralalero.jpg  | Tralala    | Iconic brainrot meme   |
| teddy.jpg      | Teddy Bear | Classic 3D plush toy   |

> 📌 For best experience, print the images or display them clearly on a screen.

---

## 🛠 Tech Stack

| Technology | Role               |
|-----------|--------------------|
| MindAR    | AR tracking engine |
| Three.js  | 3D rendering       |
| GLTF/GLB  | 3D models          |
| GitHub Pages | Web hosting    |

---

## 📁 Project Structure
```
PrajwalBendre/
├── images/               # AR markers
├── tung/                # Tung Tung 3D model
├── trala/               # Tralala 3D model
├── teddy_bear/          # Teddy Bear 3D model
├── libs/                # Optional libraries
├── sound/               # Optional audio files
├── targets.mind         # Compiled AR tracking file
├── index.html           # Main WebAR application
├── LICENSE
└── README.md
```

---

## 🔧 How It Works
1. **MindAR** detects flashcard images through your device camera.
2. **Three.js** overlays the corresponding 3D model.
3. Models are animated and rendered in real-time.
4. User experiences a seamless AR interaction in the browser.

---

## ➕ Adding New Characters
1. Add your `.gltf` model in a new folder.
2. Add its target image to `/images`.
3. Rebuild `targets.mind` using the MindAR compiler tool.
4. Update `MODELS_CONFIG` in `index.html`:
```js
{
  name: 'Your Character',
  folder: './your_folder',
  file: 'scene.gltf',
  scale: 1.0,
  rotation: 0.01
}
```

---

## 🐛 Troubleshooting

| Problem         | Solution                                      |
|----------------|-----------------------------------------------|
| Camera blocked | Enable camera permissions                     |
| No model shown | Check folder paths and console errors         |
| No AR tracking | Use printed/clear images with good lighting   |

---

## 📝 License
This project is licensed under the **MIT License**.

---

## 🤝 Contributing
Pull requests are welcome! You can:
- Add new meme characters
- Improve animation
- Enhance UI/UX

---

## 📧 Contact
**Author:** Vishwesh Pagi  
🔗 GitHub: https://github.com/vishweshvpagi  
🔗 LinkedIn: linkedin/vishweshvpagi

---

⭐ *If you enjoyed this project, please give it a star!*
**Made with 💻 and ☕ — turning memes into 3D experiences**
