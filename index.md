<!-- === UCSC GENOME BROWSER TUTORIAL HOMEPAGE === -->
<style>
/* Layout grid */
body {
  display: flex;
  font-family: "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  line-height: 1.6;
  background-color: #fafafa;
  color: #222;
}

/* Sidebar */
#sidebar {
  position: fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 260px;
  background: #0e1a40;
  color: white;
  padding: 25px 15px;
  overflow-y: auto;
  box-shadow: 3px 0 10px rgba(0,0,0,0.2);
}

#sidebar h2 {
  font-size: 1.4em;
  color: #8fd3ff;
  margin-top: 0;
}

#sidebar a {
  display: block;
  color: #d3e3ff;
  padding: 6px 10px;
  text-decoration: none;
  border-radius: 4px;
  font-size: 0.95em;
}

#sidebar a:hover {
  background: #0078d4;
  color: white;
}

/* Main content */
#content {
  margin-left: 280px;
  padding: 30px;
  max-width: 900px;
}

/* Headings */
h1, h2, h3 {
  color: #0e1a40;
}

/* Buttons */
.btn {
  display: inline-block;
  background: #0078d4;
  color: white;
  padding: 10px 20px;
  border-radius: 6px;
  text-decoration: none;
  font-weight: 600;
}

.btn:hover {
  background: #005fa3;
}
</style>

<!-- Sidebar -->
<div id="sidebar">
  <h2>🧬 UCSC Browser Tutorial</h2>
  <a href="#overview">🎯 Overview</a>
  <a href="#objectives">🧭 Learning Objectives</a>
  <a href="#prerequisites">⚙️ Prerequisites</a>
  <a href="#tutorial">🚀 Step-by-Step Tutorial</a>
  <a href="#example">🧩 Example Visualization</a>
  <a href="#discussion">🧠 Reflection</a>
  <a href="#structure">📁 Repo Structure</a>
  <a href="#citation">🧾 Citation</a>
  <a href="#contact">📬 Contact</a>
</div>

<!-- Content -->
<div id="content">

# 🧬 UCSC Genome Browser Tutorial  
**Author:** [Md Tariqul Islam (Tariq)](https://github.com/mtariqi)  
**Institution:** Northeastern University – Bioinformatics Program  
**Contact:** [tariqul@scired.com](mailto:tariqul@scired.com)

---

<div align="center">
<a href="#tutorial" class="btn">🚀 Start Learning</a>  
<a href="https://github.com/mtariqi/ucsc-genome-browser-tutorial" class="btn" style="background:#333;">View on GitHub</a>
</div>

---

## <a id="overview"></a>🎯 Overview
Welcome to the **UCSC Genome Browser Tutorial**, a step-by-step practical guide to visualizing genomic data, creating custom tracks, and sharing interactive sessions.

This tutorial is ideal for **bioinformatics students**, **researchers**, and **educators** seeking to explore genome data annotation and visualization.

---

## <a id="objectives"></a>🧭 Learning Objectives
By completing this tutorial, you will:
- Understand **BED file** format and coordinate conventions  
- Upload and visualize annotations using **custom tracks**  
- Share reproducible browser sessions via permanent URLs  
- Integrate UCSC visualization into your academic workflow  

---

## <a id="prerequisites"></a>⚙️ Prerequisites
- Web browser & Internet connection  
- (Optional) UCSC Genome Browser account  
- The file [`test.bed`](./test.bed) included in this repository  

---

## <a id="tutorial"></a>🚀 Step-by-Step Tutorial

### 1️⃣ Open the UCSC Genome Browser
Visit 👉 [https://genome.ucsc.edu](https://genome.ucsc.edu)  
Select a genome assembly, such as **hg38 (Human)**.

---

### 2️⃣ Add a Custom Track
Navigate to:  
`My Data → Custom Tracks → Add custom tracks`  
Choose the file [`test.bed`](./test.bed) and click **Submit**.

---

### 3️⃣ Visualize Your Track
After uploading, click **“Go to Genome Browser.”**  
Your BED file regions will now appear as custom annotations.

---

### 4️⃣ Share Your Session
1. Go to `My Data → Sessions`  
2. Click **Save Settings**, name your session  
3. Click **Share** to generate a permanent URL  
4. Copy this link to share or submit on Canvas  

📘 [UCSC FAQ: Sharing Sessions](https://genome.ucsc.edu/FAQ/FAQlink.html)  
🧭 [UCSC Blog: Sharing Data with Sessions and URLs](https://genome-blog.gi.ucsc.edu/blog/2021/08/13/sharing-data-with-sessions-and-urls/)

---

## <a id="example"></a>🧩 Example Visualization
![UCSC Genome Browser Screenshot](https://genome.ucsc.edu/images/gbrowser_v400.png)  
*Example of a BED custom track in UCSC Genome Browser.*

---

## <a id="discussion"></a>🧠 Discussion & Reflection
- What genomic intervals are represented in your BED file?  
- Why does UCSC use **0-based coordinates** while GFF/GTF use **1-based**?  
- How does sharing a **session URL** ensure research reproducibility?  

---

## <a id="structure"></a>📁 Repository Structure
