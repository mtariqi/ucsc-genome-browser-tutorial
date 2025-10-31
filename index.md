# 🧬 UCSC Genome Browser Tutorial  
**Author:** [Md Tariqul Islam (Tariq)](https://github.com/mtariqi)  
**Institution:** Northeastern University – Bioinformatics Program  
**Contact:** [tariqul@scired.com](mailto:tariqul@scired.com)  

---

## 🎯 Overview
Welcome to the **UCSC Genome Browser Tutorial**, an educational walkthrough designed to help students and researchers visualize and share genomic data effectively.  
This guide walks you through creating **custom tracks**, uploading **BED files**, and sharing interactive genome views with collaborators.

---

## 🧭 Learning Objectives
By the end of this tutorial, you will be able to:
- Navigate the UCSC Genome Browser efficiently.  
- Upload and visualize your own genomic annotations using **custom tracks**.  
- Share your custom sessions via permanent URLs.  
- Integrate **.bed**, **.gff**, or **.vcf** data files for reproducible research.

---

## ⚙️ Prerequisites
- A computer with internet access.  
- A UCSC Genome Browser account (optional but recommended).  
- The file [`test.bed`](./test.bed) included in this repository.

---

## 🚀 Step-by-Step Tutorial

### 1️⃣ Open the UCSC Genome Browser
Visit 👉 [https://genome.ucsc.edu](https://genome.ucsc.edu)  
Select your reference genome (e.g., **hg38** for human).

### 2️⃣ Navigate to the “Custom Tracks” Section
From the top menu, click  
`My Data → Custom Tracks → add custom tracks`.

### 3️⃣ Upload the Provided File
Click **Choose File** and select [`test.bed`](./test.bed) from this repository, then click **Submit**.

### 4️⃣ Visualize Your Track
After submission, click **“go to genome browser”**.  
You should see your custom annotations overlaid on the reference genome.

### 5️⃣ Share Your Session
1. Go to `My Data → Sessions`.  
2. Click **“Save Settings”** and give your session a name.  
3. Click **“Share”** to generate a permanent link (URL).  
4. Copy this URL to submit in Canvas or GitHub.

For detailed sharing guidance:  
📖 [UCSC FAQ: Sharing Sessions](https://genome.ucsc.edu/FAQ/FAQlink.html)  
🧭 [UCSC Blog: Sharing Data with Sessions and URLs](https://genome-blog.gi.ucsc.edu/blog/2021/08/13/sharing-data-with-sessions-and-urls/)

---

## 🧩 Example Visualization
![UCSC Genome Browser Screenshot](https://genome.ucsc.edu/images/gbrowser_v400.png)

---

## 🧠 Discussion & Reflection
- What information does the **BED** format capture?  
- How do coordinate systems differ between **UCSC (0-based)** and **GFF/GTF (1-based)** formats?  
- Why is it important to **share reproducible sessions** in bioinformatics?

---

## 📁 Repository Structure
```
ucsc-genome-browser-tutorial/
│
├── test.bed # BED file for the custom track
├── index.md # Tutorial homepage (this file)
├── README.md # Repository overview
└── assets/ # (optional) screenshots, diagrams
```


---

## 🧾 Citation & References
If you use this tutorial in your course or research, please cite:

> Islam, M. T. (2025). *UCSC Genome Browser Tutorial for Bioinformatics Education.* GitHub Repository: [https://github.com/mtariqi/ucsc-genome-browser-tutorial](https://github.com/mtariqi/ucsc-genome-browser-tutorial)

---

## 📬 Contact
If you encounter any issues or would like to contribute to this tutorial, feel free to open an issue or contact me via email:  
📧 [tariqul@scired.com](mailto:tariqul@scired.com)

---

**🧬 Happy Exploring the Genome!**  
*Developed with 💙 for the Northeastern Bioinformatics Community.*
