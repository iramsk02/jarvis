
# 🧠 Jarvis - A Python Voice Assistant

Jarvis is a voice-activated virtual assistant built using Python that mimics the functionality of smart assistants like Alexa or Google Assistant. It supports real-time voice recognition, text-to-speech feedback, web search, file access, news updates, music playback, and OpenAI-powered conversation.

---

## 🚀 Features

- 🎤 **Voice Activation with "Jarvis" Wake Word**
- 🗣️ **Speech Recognition using Google's Speech API**
- 🧠 **AI-Powered Responses via OpenAI GPT-3.5**
- 🔈 **Text-to-Speech with gTTS and Pygame**
- 🌐 **Opens popular websites like Google, YouTube, Facebook, LinkedIn**
- 📰 **Fetches Top News Headlines via NewsAPI**
- 🎵 **Plays music via custom music library URLs**
- 📄 **Opens Local Files like PPTs, PDFs, and Videos**

---

## 🛠️ Tech Stack

- Python 3
- `speech_recognition`
- `gTTS`
- `pygame`
- `pyttsx3`
- `requests`
- `openai`
- `webbrowser`
- `os` module

---

## 📁 Project Structure

```bash
.
├── client.py              # Client-side logic (optional/extendable)
├── main.py                # Main assistant logic
├── musicLibrary.py        # Contains a dictionary of song name → link
├── requirements.txt       # All required dependencies
````

---

## ⚙️ Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/iramsk02/jarvis-virtual-assistant.git
   cd jarvis-virtual-assistant
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Add Your API Keys**

   * Replace `<Your Key Here>` in `main.py` with:

     * Your **OpenAI API Key**
     * Your **NewsAPI.org Key**

4. **Configure Local File Paths**
   Update the following paths in `main.py`:

   ```python
   ppt_file_path = "path_to_induction_ppt.pptx"
   pdf_file_path = "path_to_induction_pdf.pdf"
   video_file_path = "path_to_induction_video.mp4"
   ```

5. **Run the Assistant**

   ```bash
   python main.py
   ```

---

## 🎮 Voice Commands You Can Try

* `"Jarvis"` – Activates the assistant
* `"Open Google"` – Opens Google in your browser
* `"Play [song]"` – Plays a song from your custom musicLibrary
* `"News"` – Fetches and reads headlines aloud
* `"Open induction ppt"` – Opens a local presentation file
* `"Open induction pdf"` – Opens a local PDF file
* `"Open induction video"` – Plays a local video (kulgeet)
* `"What's the weather?"` – Example AI-based response

---

## 🧠 Sample AI Query Flow

When the command doesn't match a built-in action, it is passed to OpenAI:

```python
# Example
User: "What is the capital of France?"
Jarvis (via GPT): "The capital of France is Paris."
```

---


## 📌 Notes

* Use a quiet environment for accurate speech recognition.
* GPT-3.5 API usage may incur cost; manage your OpenAI usage limits accordingly.
* This is a hobby project. Extend it with GUI, NLP, email support, etc.

---

## 🤝 Contribution

Feel free to fork this project and submit a pull request. Suggestions, issues, or feature requests are welcome!

---

## 🧑‍💻 Author

**Iram Saba Khan** – [@iramsk02](https://github.com/iramsk02)

---
