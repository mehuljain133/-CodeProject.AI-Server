# CodeProject.AI Server  
### ⚡ Self-Hosted AI Microserver Platform (2026 Edition)

**Maintained & Packaged by: Mehul Jain**  
© 2026 Mehul Jain — Open Source AI Infrastructure

---

## 🚀 Overview

**CodeProject.AI Server** is a standalone, self-hosted, ultra-fast, free and Open Source Artificial Intelligence microserver designed for:

- Any platform  
- Any programming language  
- Any AI module  
- Any developer workflow  

It runs entirely **locally**, requires **no cloud dependency**, and performs all inference **on-device**, meaning:

✅ No off-device transfer  
✅ No external network calls  
✅ Full privacy and control  
✅ Instant AI enablement inside your apps  

---

# ✨ Why This Exists

AI is no longer optional — it is the next foundation of software development.

This project was built for three reasons:

### 1. AI for Every Developer
AI programming should be approachable, fun, and practical.  
This project exists as a learning tool, a playground, and a production-ready service.

### 2. No More Dependency Hell
Frameworks, models, runtimes, GPU support, versions…  
We handle the complexity so you can focus on building.

### 3. No Paid API Lock-In
AI should not require expensive subscriptions or vendor lock-in.  
This microserver gives you full AI capability for free.

---

# ⚡ Quick Start (Developer Mode)

## Running and Debugging Locally

### Step 1 — Clone Repository
Download the source code into your workspace.

### Step 2 — Development Environment
Recommended tools:

- Visual Studio Code  
- Visual Studio 2019+  

### Step 3 — Install Dependencies
Run the setup script inside:

```

/devops/install

````

### Step 4 — Optional: Pull AI Modules
Use the module cloning script to pull all supported modules.

### Step 5 — Debug and Run
Launch the front-end server and begin testing instantly.

---

# 🧠 Using the API in Your Application

Example: Scene Detection with JavaScript

```html
<html>
<body>
<h2>Scene Detection Demo</h2>

<input id="image" type="file" />
<input type="button" value="Detect Scene" onclick="detectScene(image)" />

<script>
function detectScene(fileChooser) {
    var formData = new FormData();
    formData.append('image', fileChooser.files[0]);

    fetch('http://localhost:32168/v1/vision/detect/scene', {
        method: "POST",
        body: formData
    })
    .then(response => {
        if (response.ok) response.json().then(data => {
            console.log(`Scene: ${data.label}`);
            console.log(`Confidence: ${data.confidence}`);
        });
    });
}
</script>

</body>
</html>
````

---

# 📦 What’s Included

CodeProject.AI Server provides three major layers:

---

## 1. 🌐 REST API Microserver

A lightweight HTTP service that receives requests and routes them to AI modules.

* Runs as a local web service
* Works with any programming language
* Designed for production deployment

---

## 2. 🧩 Backend AI Analysis Services

The intelligence layer.

All processing happens locally:

* No cloud calls
* No data leaks
* GPU acceleration supported
* Modular architecture

---

## 3. 📂 Full Source Code

Everything is included.

You can:

* Modify modules
* Add new AI services
* Build custom inference pipelines
* Extend the platform freely

---

# 🔥 Capabilities (2026 Maxed Feature Set)

CodeProject.AI can run any AI module your imagination creates.

Current built-in module categories include:

---

## 🤖 Generative AI

* Large Language Models for text generation
* Multi-modal AI ("describe this image")
* Text-to-Image generation pipelines
* AI assistant integration modules

---

## 👁 Vision Intelligence

* Object Detection (custom models supported)
* Face Detection and Recognition
* Scene Classification
* Background Removal
* Background Blur
* Image Enhancement / Super Resolution

---

## 📝 Natural Language Processing

* Text Summarization
* Sentiment Analysis
* Keyword Extraction
* Document Intelligence Modules

---

## 🔊 Audio Intelligence

* Sound Classification
* Audio Event Detection
* Voice-based module expansion support

---

# 🎯 Project Goals

### ✅ Promote AI Development

This is an explorer, learning platform, and AI service framework for developers.

### ✅ Make AI Development Easy

Not because AI is hard — but because AI ecosystems are messy.
This system provides structure and simplicity.

### ✅ Focus on Practical Use-Cases

We prioritize clarity and usefulness over overwhelming complexity.

### ✅ Empower the Developer Community

The platform grows through community contributions and shared innovation.

---

# 🖥 Supported Platforms & Acceleration

This release supports:

* Windows 10+
* Ubuntu 22.04+
* Debian
* macOS (Intel + Apple Silicon)

Hardware acceleration support includes:

* CPU Inference
* CUDA (Windows + Linux)
* DirectML (Windows)
* Apple Silicon GPU Support
* RockChip NPUs
* Coral AI TPU Support

(Module support depends on implementation.)

---

# 🆕 Latest Release Notes (2026)

### Version 2.9 Highlights

* Upgraded to **.NET 9**
* Expanded Linux compatibility
* Improved CUDA 12 support
* Windows + Linux GPU performance fixes
* macOS arm64 improvements
* Installer reliability upgrades
* Developer environment stabilization

---

# 🎨 UI & Developer Experience (Maxed 2026)

This project is designed with modern usability in mind:

✅ Clean REST-first architecture
✅ Plug-and-play AI module system
✅ Developer-friendly debugging
✅ Simple local install workflow
✅ Expandable UI dashboard ready
✅ Future-ready AI editor integration

---

# 📌 Maintainer

**Mehul Jain**
Open Source AI Microserver Infrastructure
2026 Edition Release

---

# 📜 License

This project is distributed under Open Source licensing.
Third-party notices and compliance documentation are included inside the repository.

---