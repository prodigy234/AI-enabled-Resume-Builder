
# 🧠 AI Resume Builder

**AI Resume Builder** is a modern and interactive Streamlit web app that helps users generate professional, beautifully formatted resumes in `.docx` and `.pdf` formats — within minutes.

Designed for professionals, job seekers, and students, the app offers smart resume customization with an intuitive user interface and real-time preview generation.

---

## 🚀 Features

- 📝 Fillable form for personal details, education, skills, work experience, and more.
- 📄 Automatically generates both Word (.docx) and PDF (.pdf) resumes.
- 🎨 Modern UI with custom CSS styling for enhanced user experience.
- 🧠 AI-assisted sectioning and formatting.
- 🔒 Runs locally and ensures your resume data stays private.
- 📥 Download buttons for both file types.
- 🧾 Clean layout and intuitive sidebar navigation.

---

## 📸 Screenshot

*(Optional: Add screenshots of the app here)*

---

## 🛠️ Tech Stack

| Technology       | Usage                                |
|------------------|---------------------------------------|
| Python           | Backend logic and resume generation   |
| Streamlit        | Web interface                         |
| python-docx      | Word (.docx) resume generation        |
| FPDF             | PDF resume generation                 |
| Pillow (PIL)     | Image handling                        |
| HTML/CSS         | Custom UI Styling                     |

---

## 📦 Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/ai-resume-builder-ultra.git
cd ai-resume-builder-ultra
```

### Install Dependencies

```bash
pip install streamlit python-docx fpdf Pillow
```

---

## ▶️ Running the App

Run the following command in your terminal:

```bash
streamlit run app.py
```

This will launch the app in your default web browser.

---

## 💡 How to Use

1. Enter your personal details from the sidebar.
2. Fill in your professional summary, skills, experience, education, certifications, and leadership.
3. Click the `🚀 Generate My Resume` button.
4. Download your resume as a `.docx` or `.pdf` file using the download buttons.

---

## 📁 File Structure

```
├── app.py                     # Main Streamlit App
├── My image6.jpg              # Developer Image (for footer)
├── requirements.txt           # Package dependencies
└── README.md                  # This file
```

---

## 🧠 Sample Code Snippet

```python
if st.button("🚀 Generate My Resume"):
    final_doc = generate_resume()
    docx_buffer = BytesIO()
    final_doc.save(docx_buffer)
    docx_buffer.seek(0)
    pdf_buffer = generate_pdf()
    st.success("🎉 Your resume is ready!")
    st.download_button("⬇️ Download .docx Resume", docx_buffer, file_name=f"{name.replace(' ', '_')}_Resume.docx")
    st.download_button("⬇️ Download .pdf Resume", pdf_buffer, file_name=f"{name.replace(' ', '_')}_Resume.pdf")
```

---

## 👨‍💻 About the Developer

**Kajola Gbenga**

📇 Certified Data Analyst | Certified Data Scientist | Certified SQL Programmer | Mobile App Developer | AI/ML Engineer

- 🔗 [LinkedIn](https://www.linkedin.com/in/kajolagbenga)  
- 📜 [Certifications & Licences](https://www.datacamp.com/portfolio/kgbenga234)  
- 💻 [GitHub](https://github.com/prodigy234)  
- 🌐 [Portfolio](https://kajolagbenga.netlify.app/)  
- 📧 Email: k.gbenga234@gmail.com

---

## ✅ License

This project is open-source and available under the [MIT License](LICENSE).

---

## 💬 Feedback & Contributions

Pull requests and issues are welcome. If you'd like to contribute, please fork the repo and submit a PR.

---
