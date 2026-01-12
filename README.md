
# WhatsApp Chat Analyser

A **Streamlit-based web application** that analyzes exported WhatsApp chat files and provides detailed statistics, visualizations, emoji insights, timelines, heatmaps, and more.

## 🙏 Acknowledgment

This project was inspired by various data analytics and visualization resources available in the open-source community.  
Special thanks to the following:

- Streamlit community for excellent UI documentation
- Pandas contributors for powerful data handling capabilities
- Matplotlib/Seaborn maintainers for visualization support
- WordCloud & urlextract developers for helpful libraries

We also acknowledge WhatsApp™ as the source of exported chat data.  
This project is **not affiliated, associated, authorized, or endorsed by WhatsApp or Meta Platforms, Inc.**

## 📚 API References

### ✅ Streamlit
Used to build the web-based UI.
- Documentation: https://docs.streamlit.io/
- Common APIs used:
  - `st.sidebar.file_uploader()`
  - `st.sidebar.selectbox()`
  - `st.button()`
  - `st.pyplot()`
  - `st.dataframe()`

---

### ✅ Pandas
Used for data cleaning, grouping, and time-series extraction.
- Documentation: https://pandas.pydata.org/docs/
- Common APIs used:
  - `pd.DataFrame()`
  - `df.groupby()`
  - `df.value_counts()`
  - `df['col'].dt.year/month/day/...`

---

### ✅ Matplotlib / Seaborn
Used to visualize timelines, bar charts, and heatmaps.
- Matplotlib Docs: https://matplotlib.org/stable/
- Seaborn Docs: https://seaborn.pydata.org/
- Common APIs:
  - `plt.subplots()`
  - `ax.plot()`
  - `ax.bar()`
  - `sns.heatmap()`

---

### ✅ WordCloud
Used to generate WordCloud visuals from chat text.
- Docs: https://amueller.github.io/word_cloud/
- Common APIs:
  - `WordCloud.generate()`

---

### ✅ URLExtract
Used to detect links inside chat messages.
- Documentation: https://pypi.org/project/urlextract/
- Common APIs:
  - `URLExtract().find_urls()`

---

### ✅ Emoji
Used to extract emojis from text.
- Documentation: https://pypi.org/project/emoji/
- Common APIs:
  - `emoji.UNICODE_EMOJI`



## Screenshots
<img width="1919" height="1079" alt="Screenshot 2025-11-08 235817" src="https://github.com/user-attachments/assets/455ffd1d-87ec-4191-a8f7-96bf8e688f0f" />
<img width="1915" height="1079" alt="Screenshot 2025-11-09 000010" src="https://github.com/user-attachments/assets/07ebd947-1297-4dc1-bb20-6f12923aed73" />
<img width="1913" height="1075" alt="Screenshot 2025-11-09 000001" src="https://github.com/user-attachments/assets/75ef0aab-b6ed-474d-a02b-dedf8419d094" />
<img width="1918" height="1079" alt="Screenshot 2025-11-08 235951" src="https://github.com/user-attachments/assets/1baed380-abf9-43f1-8566-0729e06441c0" />
<img width="1919" height="1077" alt="Screenshot 2025-11-08 235940" src="https://github.com/user-attachments/assets/fd2b5840-b86a-4e85-ae6e-6498998118bb" />

## Appendix
WhatsApp Chat Export Format

The analyzer works on exported WhatsApp chats in text (.txt) format.
Typical line structure:

DD/MM/YYYY, HH:MM - Username: Message content


Example:

12/03/2023, 21:15 - John: Hey, what's up?
12/03/2023, 21:16 - Emily: All good!


Media placeholder example:

<Media omitted>


⚠️ The export must be without media.

Data Columns Generated


Reference Formatting Patterns

Regex used for splitting messages:

\d{1,2}/\d{1,2}/\d{2,4},\s\d{1,2}:\d{2}\s-\s


Datetime conversion:

format='%d/%m/%Y, %H:%M - '

Credits for Libraries

Streamlit

Pandas

Matplotlib

Seaborn

URLExtract

WordCloud

Emoji
## Features

Upload WhatsApp chat text file
View total messages, words, media shared, and links shared
Monthly & daily chat timeline
Activity heatmap (day + hour)
Busiest day & month
User-wise stats (Most active users)
Word cloud generation
Most common words
Emoji usage frequency + pie chart
Works for individual users or an entire group
## Documentation

This application processes exported WhatsApp chat files (.txt) and provides analytic insights through an interactive Streamlit interface.

🔹 Workflow

User uploads chat file.
The text is parsed to extract the timestamp, sender, and message content.
Data is structured using Pandas.
Key metrics and visualizations are generated.
Results are presented in an intuitive dashboard.


# Hi, I'm Aditya Verma! 👋


## 🚀 About Me
I'm a Btech II Year CSE AIML Student...


## Installation

### 1️⃣ Clone the repository
--bash
git clone
    https://github.com/aditya484/WhatsAppChatAnalyser.git

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

http://10.109.126.193:8501

## 🛠 Skills
Python, Pandas, Streamlit, Matplotlib/Seaborn ...

👩‍💻 I'm currently in II Year of Btech CSE AIML...

📫 How to reach me... adityalkverma484@gmail.com
😄 Pronouns... He/Him
⚡️ Fun fact... It was my first Project


## Authors

- [Aditya Verma](https://github.com/aditya484)
- [Divyam Sinha]()
- [Mark James] ()
## License

[MIT](https://choosealicense.com/licenses/mit/)


## Lessons Learned

- Handling Raw Unstructured Text
- Importance of Data Cleaning
- Working wuth Date and Time Data
- Visual Representaion of Data
- User- Centered Interface
- Moular Benfits (preprocessor.py, helper.py, app.py)
    Code maintainable
    Easier debugging
    Faster extension
- Future Enhancements Identified
    Sentiment analysis
    Multi-language support
    Chat comparison support
    Better error handling

🔹 Learning Resources
Topic	         Link
Streamlit	    https://docs.streamlit.io
Pandas      	https://pandas.pydata.org
Matplotlib   	https://matplotlib.org
Seaborn     	https://seaborn.pydata.org
WordCloud	    https://github.com/amueller/word_cloud

Emoji	        https://pypi.org/project/emoji/


## Tech Stack

**Client:** Streamlit UI Components, MAtplotlib, Seaborn

**Server:** Pyhton, Pandas, Regex(re), URLextract, emoji

