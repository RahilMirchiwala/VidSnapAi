# 🎬 VidSnapAI

**VidSnapAI** is an AI-powered tool that converts images and text descriptions into short video reels automatically.  
It uses **Flask** for the web interface and **FFmpeg** for video generation, combining uploaded images with AI-generated voiceovers.

---

## 🚀 Features

- 📤 Upload multiple images  
- 📝 Add a text description for the video  
- 🔊 Converts text to speech using AI  
- 🎥 Combines images + audio into vertical video reels  
- 🖼️ View generated reels in a built-in gallery  

---

## 🧠 How It Works

1. User uploads images and provides a short description.  
2. The app stores the data inside a unique folder.  
3. The background process reads the description, generates an audio narration, and uses **FFmpeg** to combine the images and audio into a short video.  
4. The final reel is saved inside the `static/reels` folder and shown in the gallery page.

---

## ⚙️ Installation

### Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate       # for Linux/Mac
venv\Scripts\activate          # for Windows
```
### Install dependencies
```bash
pip install flask werkzeug gtts
```
### Install FFmpeg
Make sure FFmpeg is installed and available in your system PATH.
Check installation by running:
```bash
ffmpeg -version
```
### ▶️ Usage
```bash
python main.py
```
Then open http://127.0.0.1:5000 in your browser.

### Run the background process:
```bash
python generate_process.py
```
💡 Keep this running alongside your Flask app to automatically process uploaded files into reels.

## 📁 Example Workflow

1. Open the `/create` page in your browser.  
2. Upload your images.  
3. Add a text description (for narration).  
4. Wait a few seconds while the system generates your video reel.  
5. View all generated videos on the `/gallery` page.

---

## 🧩 Dependencies

- **Python 3.8+**  
- **Flask**  
- **Werkzeug**  
- **FFmpeg**  
- **gTTS** (for text-to-speech)

---

## 🧠 Future Improvements

- ✅ Progress tracking for video generation  
- ✅ Advanced AI voice synthesis integration  
- ✅ Background music support  
- ✅ User authentication and personal gallery  

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use and modify it.

---

## 💡 Author

**👨‍💻 Rahil Mirchiwala**  
🎓 B.Tech CSE | MERN Stack Developer | Data Science Enthusiast  
🔗 [LinkedIn]([https://www.linkedin.com/in/rahil-mirchiwala])

