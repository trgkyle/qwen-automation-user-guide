[![Download Here](https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge)](https://chromewebstore.google.com/detail/qwen-automation-auto-qwen/gfolnjohlchemjcllgjgbfhaafdpkenk)

# 🚀 Qwen Automation v1.0.2 - chat.qwen.ai AI Automation [![Tiếng Việt](https://img.shields.io/badge/Tiếng%20Việt-green)](README_vi.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md)

**Qwen Automation** is a powerful productivity tool that automates your creative workflow on Qwen AI (`chat.qwen.ai`). Instead of manually copying and entering prompts one by one, you can queue dozens or hundreds of prompts to automatically generate videos and images at scale.

-----

## ✨ Key Features

* **🚀 Batch Processing:** Queue large sets of prompts and let the extension handle the automation process, including prompt submission and generation.
* **🧩 Workflow (visual drag-and-drop editor):** Connect prompts, images and generators on a canvas — e.g. generate images, then turn those images into videos automatically. Save several workflows, run one node or all of them, import/export them as files.
* **🎬 Text-to-Video Automation:** Convert text descriptions into high-quality videos automatically.
* **🎬 Frame-to-Video (Image-to-Video):** Animate static images using prompts to create dynamic motion effects. Supports using start frames or start & end frames.
* **🎬 Ingredients-to-Video:** Feed multiple image inputs (up to 10) per prompt to generate rich composite videos.
* **🖼️ Text-to-Image Batching:** Generate multiple high-quality images with full support for various aspect ratios.
* **🖼️ Image-to-Image:** Enhance or modify existing images using AI and customized prompts.
* **⚙️ Professional Automation Controls:**
    * **Concurrent Prompts:** Run multiple prompts at the same time to accelerate your workflow.
    * **Random Delays:** Introduce smart delays between prompt submissions to handle rate limits gracefully.
    * **Auto Download:** Automatically download generated images and videos upon completion.
    * **Auto Rename:** Automatically rename downloaded files based on settings.
* **📊 Side Panel Queue Monitoring:** Monitor progress with an active queue, delay count-down, and a visual status bar in the Chrome Side Panel.
* **📂 Organized File Management:** Download files into customized subfolders based on your projects.
* **🌐 Multi-language Support:** English, Tiếng Việt, 中文, 한국어, Español, 日本語.

-----

## 📥 Installation

### Method 1: Chrome Web Store (Recommended)
1. Visit the [Chrome Web Store](https://chromewebstore.google.com/detail/qwen-automation-auto-qwen/gfolnjohlchemjcllgjgbfhaafdpkenk) and click **Add to Chrome**.

---

## 📖 User Guide

### Getting Started

1. **Navigate to Qwen AI**
   - Open [chat.qwen.ai](https://chat.qwen.ai).
   - Ensure you are logged into your Qwen account.

2. **Open the Extension**
   - Click the extension icon in the Chrome toolbar. We recommend pinning it for quick access.
   - The side panel will open.

3. **Configure Batch Settings**
   - In the **Control** tab, you can set the **Save to folder** name to organize your downloads.
   - In the **Setting** tab, customize your **Concurrent Prompts**, **Random Delay**, model selections, and download options.

4. **Select a Mode**
   - Click one of the mode buttons: **Text to Video**, **Frame to Video**, **Ingredients to Video**, **Text to Image**, or **Image to Image**.

---

### Mode Instructions

#### 1. Text-to-Video Mode
1. Select **Text to Video** mode.
2. Enter prompts in the text box (separate prompts with a **blank line**).
3. Alternatively, click **Upload .txt file** or **Upload .xlsx / .csv** to import prompts.
4. Click **Run** to start generating videos.

**Example Prompt:**
```
A cozy cabin in the snow with a warm fire crackling inside.
The camera moves slowly through the window.

A high-tech sci-fi command center with holograms glowing in the dark.
A close-up shot of a holographic map.
```

#### 2. Frame-to-Video Mode
1. Select **Frame to Video** mode.
2. Drag & drop or click to upload your source image(s).
3. Enter your prompts (separated by blank lines).
4. Configure whether to use a **Start frame only** or **Start frame and End frame** in Settings.
5. Click **Run**.

#### 3. Ingredients-to-Video Mode
1. Select **Ingredients to Video** mode.
2. Upload multiple asset images (up to 10 per prompt).
3. Toggle **Auto-add character images** to automatically match images to prompt names based on their filenames.
4. Input prompts (separated by blank lines) and click **Run**.

#### 4. Text-to-Image Mode
1. Select **Text to Image** mode.
2. Enter detailed prompts separated by blank lines.
3. Configure the desired **Default Aspect Ratio** in Settings.
4. Click **Run**.

#### 5. Image-to-Image Mode
1. Select **Image to Image** mode.
2. Upload the source image(s) you wish to modify.
3. Enter text prompts describing the modifications or style adjustments.
4. Click **Run**.

### 🧩 Workflow (Visual Drag-and-Drop Editor)

Workflow is a visual drag-and-drop editor for flows with several steps — for example: generate a few images, then use those images to make videos, then continue each video with another prompt. It opens in its own window and runs on your open chat.qwen.ai tab.

#### Open it

* Click **Workflow** in the Control tab (bottom row).
* Already typed prompts or uploaded images in the side panel? Hover **Workflow** and click **Convert to workflow**: your prompts, each prompt's mode and your images become nodes in the editor, ready to run.

#### The screen

| Area | What it holds |
| :--- | :--- |
| **Left** | **Nodes** (click or drag one onto the canvas) and **Your workflows** (all saved workflows) |
| **Top bar** | The canvas tools: Undo/Redo, **Auto arrange**, fit view, **Example**, clear. On the right: the **Details** button, **Shortcuts** and the chat.qwen.ai tab status |
| **Canvas** | Your nodes. Top-left: **Run all** (and **Stop** while running) and **Enable background mode** |

The **Details** button shows what needs attention: **Issues (n)** in red/yellow when something blocks a run, **Running 3/8** while generating. Click it to open a panel with the issues (click one to jump to the node), live progress, the run plan and the settings it uses.

#### Nodes

| Node | What it does |
| :--- | :--- |
| **Enter prompt** | One or more prompts, separated by a **blank line** |
| **Upload image** | Your images (drop files on it). Hover an image: 🔍 to view it larger, ✕ to remove it, the grip in the corner to drag it to another position. The order (or the sort menu) decides which prompt gets which image |
| **Generate Image** | Text to Image, or Image to Image when images are connected. Options: **Image Mode per Prompt**, **Max Input Images per Prompt**, **Auto-add character images** |
| **Generate Video** | Text to Video, or with images connected **Frame to Video** / **Components to Video**. Options: **Video Mode per Prompt**, images per prompt (shared with the side panel settings), **Auto-add character images** (Components to Video) |

Generate nodes are named automatically from their first prompt (`image_…` / `video_…`). Each prompt row shows the images it will receive, so you can check before running. Their preview takes the **aspect ratio** from the settings (a 9:16 node is narrower and taller).

#### Connect nodes

Drag from the round handle on the right of a node and **drop it anywhere on the other node** — the right input is picked for you. Nodes that accept the connection light up while you drag.

| From | To | Meaning |
| :--- | :--- | :--- |
| Enter prompt | Generate Image / Generate Video | The prompts to generate |
| Upload image | Generate Image / Generate Video | Reference images, start frames or components |
| Generate Image | Generate Image / Generate Video | The **generated images** become that node's input (it runs after the images are ready) |
| Generate Video — **last frame** output | Generate Video | The next video **continues from the last frame** of this one |
| Generate Video — **last frame** output | Generate Image | The **last frame** of each video becomes an input image (it runs after the video is ready) |

#### Run

* **Run all** (top-left, or `Ctrl/⌘ + Enter`) runs the whole workflow in the right order: nodes waiting for generated images start automatically once those images exist.
* If **Run all** is disabled, the top bar shows **Issues (n)**: click it to see what to fix.
* Each Generate node also has its own **Run** button to run only that node. It is disabled until the nodes it depends on have finished (hover to see why).
* **Stop** cancels what is still running.
* While running, the connections into the node that is generating light up and flow, so you can see where the workflow is.

> ⚠️ **Chrome pauses chat.qwen.ai when its tab isn't visible** (for example when the workflow window covers it full screen). Click **Enable background mode** (under **Run all** in the workflow, or in the side panel), then pick the chat.qwen.ai tab in Chrome's dialog. This shares the chat.qwen.ai tab (nothing is recorded or sent anywhere) so it keeps generating behind other windows. The green **Running in background** badge shows it's on; click ✕ to stop it.

#### Results

Results appear inside each Generate node. Hover a result: 🔍 opens it large, ✕ removes it (the eraser clears all results of the node). Videos play on hover. Files are still downloaded as usual.

The next node uses the **first result of each prompt**. To choose which one, drag a result by the grip in its top-left corner onto another result to swap them (images and videos).

#### Manage workflows

Under **Your workflows** (left): **New**, **Import**, and for each workflow the **⋯** menu — **Rename** (or double-click the name), **Duplicate**, **Export**, **Delete**. Everything is saved automatically.

* **Export** downloads a `.json` file. It starts with `//` comment lines that describe every node, property and connection, so you can give the file to an AI assistant and ask it to write new workflows. The comment lines are removed on import.
* **Import** a file with the button, or simply **drag the `.json` file onto the canvas**.

#### Editing shortcuts

Click **Shortcuts** in the top bar (or press `?`) to see them all.

| Action | Keys |
| :--- | :--- |
| Undo / Redo | `Ctrl/⌘ + Z` / `Ctrl/⌘ + Shift + Z` |
| Copy / Cut / Paste nodes (also into another workflow) | `Ctrl/⌘ + C / X / V` |
| Duplicate selection | `Ctrl/⌘ + D` |
| Select all / Add to selection / Box select | `Ctrl/⌘ + A` / `Ctrl/⌘ + click` / `Shift + drag` |
| Auto arrange | `Shift + A` |
| Delete selected | `Delete` |
| Run all / Run in background | `Ctrl/⌘ + Enter` / `Ctrl/⌘ + Shift + Enter` |

---

## ⚙️ Settings Configuration

Access the **Setting** tab in the side panel to fine-tune automation behavior:

* **Default Mode:** Set the default creation mode.
* **Default Aspect Ratio:** Choose from 16:9, 9:16, 1:1, 3:4, or 4:3.
* **Outputs per Prompt:** Control the number of outputs generated per prompt (1 to 4 for video).
* **Outputs Image per Prompt:** Specify image batch counts (from 1 up to 50).
* **Concurrent Prompts:** Choose how many prompts to run simultaneously (1 to 6 prompts).
* **Random Delay:** Set standard random wait time between handling prompts.
* **Video Model & Image Model:** Choose the specific AI models for video/image generation.
* **Default Video/Image Options:** Set duration/stretching mode (e.g., 5 seconds or 5 seconds concat to stitch videos; New Image or Edit Image/chain mode for images).
* **Max Input Images:** Configure maximum asset limits for Frame-to-Video, Ingredients-to-Video, and Image-to-Image.
* **Max Retries on Failure:** Specify retries (1 to 20) if generation fails.
* **Auto Download Quality:** Set auto-download quality (No Download, 1080p for videos, 1k for images).
* **Download Settings:** Organizes generated outputs into separate project subfolders under Chrome's Download directory.
* **Language:** Switch between English, Tiếng Việt, 中文, 한국어, Español, and 日本語.

---

## 💡 Tips & Best Practices

1. **Handling Rate Limits:** If Qwen limits your account activity, increase the **Random Delay** between prompts.
2. **Optimal Concurrency:** Start with 1 concurrent prompt and slowly increase it based on how your Qwen account performs.
3. **Stitching Videos:** Use the **5s concat** option in settings to combine consecutive prompt outputs into a single, continuous video.
4. **Auto-naming & Folders:** Name your project folder in the Control tab so that all files are grouped together cleanly.

---

## 🔧 Troubleshooting

| Issue | Solution |
| :--- | :--- |
| **Extension Not Active** | Make sure you are on [chat.qwen.ai](https://chat.qwen.ai). Refresh the page if needed. |
| **Generation Errors** | Click the **Fix Error** button in the extension. The extension will automatically retry up to your configured Max Retries. |
| **Downloads Not Working** | Turn **OFF** the "Ask where to save each file before downloading" setting in your Chrome browser settings. |
| **Authentication Issues** | Verify you are signed in to both `chat.qwen.ai` and your extension plan account (via the Plan Banner). |
| **Workflow: generation stays at "Generating" forever** | Chrome paused the hidden chat.qwen.ai tab. Turn on **Enable background mode** (or **Run in background**), or keep chat.qwen.ai visible. |
| **Workflow: a node's Run button is disabled** | Hover it: run the node it depends on first, or fix the issue shown (e.g. no prompt connected). |
| **Workflow: Run all is disabled** | Click **Issues (n)** in the top bar to see what to fix; click an issue to jump to its node. |
| **Workflow: "No chat.qwen.ai tab found"** | Open [chat.qwen.ai](https://chat.qwen.ai) in a tab (the green dot in the top bar shows it's connected). |

---

## 🔒 Privacy & Data

* **Local Processing:** All automation actions and page navigation scripts run locally on your browser sandbox.
* **No External Storage:** We do not collect, monitor, or store your prompts, uploaded images, or generated files.
* **Secure Sync:** Settings are saved directly within your Chrome local storage and synced across tabs automatically.

---

## 📞 Support

- **Author:** Trường Nguyễn
- **Website:** [kylenguyen.me](https://kylenguyen.me)
- **Feedback:** Use the **Report Bug** tab in the extension to copy debug logs and send them to our support channels.

---

## 📦 Version

Current version: **1.0.2**

---

## 📜 License

Copyright © 2026 **Trường Nguyễn**. All Rights Reserved.

This software is proprietary. Unauthorized copying, modification, or distribution is prohibited.

---

**Made with ❤️ by Trường Nguyễn**
