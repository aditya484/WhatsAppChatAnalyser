# WhatsAppChatAnalyser

## 🚀 Features

- Upload WhatsApp chat text file
- View total messages, words, media shared, links shared
- Monthly & daily chat timeline
- Activity heatmap (day + hour)
- Busiest day & month
- User-wise stats (Most active users)
- Word cloud generation
- Most common words
- Emoji usage frequency + pie chart
- Works for individual users or entire group

## 📂 Project Structure

```
├── app.py               # Main Streamlit app
├── helper.py            # Analytics functions
├── preprocessor.py      # Chat text processing
├── stop_hinglish.txt    # Stop words for cleanup
├── README.md            # Project documentation


## 📁 How to Export WhatsApp Chat

1. Open WhatsApp
2. Go inside the chat
3. Tap **⋮ → More → Export Chat**
4. Export **without media**
5. Upload `.txt` file to the app

## 📊 Sample Outputs

- Total messages, words, media, links count
- Monthly chat trends
- Daily chat usage
- Weekly & monthly activity
- Heatmap of day & hour
- Most active members
- Word cloud
- Emoji usage table + pie chart

## 📦 Installation

### 1️⃣ Clone the repository
--bash
git clone https://github.com/yourusername/whatsapp-chat-analyzer.git
cd whatsapp-chat-analyzer

### 2️⃣ Create a virtual environment
---bash
python -m venv venv

### 3️⃣ Activate environment

**Windows**
---bash
venv\Scripts\activate

**Mac / Linux**
---bash
source venv/bin/activate


### 4️⃣ Install dependencies
---bash
pip install -r requirements.txt


> **Note:** Ensure `stop_hinglish.txt` exists in project root.

## ▶️ Run the App

---bash
streamlit run app.py


The app will open in your browser automatically.  
If not, open:

http://localhost:8501

## ✅ To-Do / Enhancements

- Add sentiment analysis
- Add PDF report export
- Multi-language support
- Better group tagging

## 🤝 Contributions

Pull requests and feature additions are welcome!  
Open an issue if you’d like to request something.

## 📄 License

MIT License

## ⭐ Support

If you like this project, please ⭐ the repository.
