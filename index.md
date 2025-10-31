# 🧬 UCSC Genome Browser Tutorial  
**Author:** [Md Tariqul Islam (Tariq)](https://github.com/mtariqi)  
**Institution:** Northeastern University – Bioinformatics Program  
**Contact:** [tariqul@scired.com](mailto:tariqul@scired.com)  

---

<div align="center">

[![Start Learning 🚀](https://img.shields.io/badge/Start%20Learning-Click%20Here-blue?style=for-the-badge)](#-step-by-step-tutorial)  
[![GitHub Repo](https://img.shields.io/badge/View%20on-GitHub-black?style=for-the-badge&logo=github)](https://github.com/mtariqi/ucsc-genome-browser-tutorial)

</div>

---

<details>
<summary><b>📚 Table of Contents (click to expand)</b></summary>

- [Overview](#-overview)  
- [Learning Objectives](#-learning-objectives)  
- [Prerequisites](#️-prerequisites)  
- [Step-by-Step Tutorial](#-step-by-step-tutorial)  
  - [1️⃣ Open the UCSC Genome Browser](#1️⃣-open-the-ucsc-genome-browser)  
  - [2️⃣ Navigate to Custom Tracks](#2️⃣-navigate-to-the-custom-tracks-section)  
  - [3️⃣ Upload the BED File](#3️⃣-upload-the-provided-file)  
  - [4️⃣ Visualize Your Track](#4️⃣-visualize-your-track)  
  - [5️⃣ Share Your Session](#5️⃣-share-your-session)  
- [Example Visualization](#-example-visualization)  
- [Discussion & Reflection](#-discussion--reflection)  
- [Repository Structure](#-repository-structure)  
- [Citation & References](#-citation--references)  
- [Contact](#-contact)

</details>

---

## 🎯 Overview
Welcome to the **UCSC Genome Browser Tutorial**, a hands-on introduction to genomic data visualization.  
This guide walks you through uploading custom data, creating shareable genome tracks, and generating reproducible sessions.  
Designed for students, researchers, and professionals learning bioinformatics visualization techniques.

---

## 🧭 Learning Objectives
By completing this tutorial, you will:
- Understand the structure of **BED files**.  
- Upload and visualize genomic features using **custom tracks**.  
- Generate and share reproducible browser sessions.  
- Integrate your findings into academic or clinical research workflows.

---

## ⚙️ Prerequisites
Before starting, make sure you have:
- Internet access.  
- A UCSC Genome Browser account (optional).  
- The file [`test.bed`](./test.bed) included in this repository.  

---

## 🚀 Step-by-Step Tutorial

### 1️⃣ Open the UCSC Genome Browser
Visit 👉 [https://genome.ucsc.edu](https://genome.ucsc.edu)  
Choose your genome assembly (e.g., **hg38** for human).

---

### 2️⃣ Navigate to the “Custom Tracks” Section
In the top menu, go to:  
`My Data → Custom Tracks → Add custom tracks`

---

### 3️⃣ Upload the Provided File
Click **Choose File**, select [`test.bed`](./test.bed), then click **Submit**.  
Once uploaded, your BED data will be parsed and ready for visualization.

---

### 4️⃣ Visualize Your Track
After submission, click **“Go to Genome Browser”**.  
Your custom regions will appear aligned with existing annotation tracks.

---

### 5️⃣ Share Your Session
To generate a link to your visualization:
1. Go to `My Data → Sessions`  
2. Click **“Save Settings”** and name your session.  
3. Click **“Share”** → copy the permanent link (URL).  
4. Paste the link in Canvas or share it with collaborators.  

For detailed guidance:  
📘 [UCSC FAQ: Sharing Sessions](https://genome.ucsc.edu/FAQ/FAQlink.html)  
🧭 [UCSC Blog: Sharing Data with Sessions and URLs](https://genome-blog.gi.ucsc.edu/blog/2021/08/13/sharing-data-with-sessions-and-urls/)

---

## 🧩 Example Visualization
![UCSC Genome Browser Screenshot](https://genome.ucsc.edu/images/gbrowser_v400.png)  
*Example of a BED custom track visualized in the UCSC Genome Browser.*

---

## 🧠 Discussion & Reflection
- What genomic regions does your BED file annotate?  
- Why does UCSC use **0-based coordinates**, and how does this affect alignment?  
- How can you use shared session URLs in reproducible research pipelines?

---

## 📁 Repository Structure
