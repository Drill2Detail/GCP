Below is the provided text converted into Markdown format for your GitHub repository. I have maintained the original wording exactly as requested, using standard Markdown headers, lists, and code blocks for readability.

# Gemini CLI: Code & Create with an Open-Source Agent

**Course Link:** [https://www.deeplearning.ai/short-courses/gemini-cli-code-and-create-with-an-open-source-agent/](https://www.deeplearning.ai/short-courses/gemini-cli-code-and-create-with-an-open-source-agent/)

## What you'll learn
* Use Gemini CLI’s agent with Model Context Protocol (MCP) and extensions to coordinate local files with cloud services like Google Workspace and Canva for multi-tool workflows.
* Automate software development tasks, including building website features, creating data dashboards, and setting up code review workflows with GitHub Actions.
* Apply Gemini CLI to tasks beyond code like generating social media content from multimedia files and organizing study materials for learning.

## About this course
Join this short course on Gemini CLI, taught by Jack Wotherspoon, Developer Advocate at Google.

Gemini CLI is an open-source agentic coding assistant that works from your terminal, giving it access to your local filesystem, development tools, and cloud services. This lets you delegate complex workflows—from building web features to creating marketing materials—through high-level instructions while the agent autonomously plans and executes multiple steps.

In this course, you’ll apply Gemini CLI to software development and creative tasks by building features for an AI conference. You’ll develop a website session catalog, create a data dashboard combining local and cloud data sources, and generate social media content from recordings. You’ll master context management, integrate MCP servers, and orchestrate across multiple services with Gemini CLI extensions.

### In detail, you’ll:
* Install Gemini CLI, explore its open-source architecture, and learn how it reasons through tasks, calls tools, and leverages the command line to power complex workflows.
* Automate coding workflows with GitHub Actions for pull request reviews and apply Gemini CLI to creative tasks like generating social media content from conference recordings and organizing multimedia study materials.
* Manage the context window with gemini.md files and extend capabilities by connecting Model Context Protocol (MCP) servers and Gemini CLI extensions to orchestrate across local files, cloud databases, and services like GitHub, Canva and Google Workspace.
* Build complete software features including a conference session catalog and an interactive data dashboard that combines local CSV files with cloud data sources—experiencing the full development workflow from research to testing.
* Use Gemini CLI as a learning tool by organizing course materials on your filesystem and grounding responses with web search for accurate, cited information.

Whether you’re prototyping applications, automating development workflows, or studying topics in agentic AI, this course gives you hands-on experience coordinating multiple tools to build faster and work more efficiently.

## Who should join?
Anyone looking to speed up development and knowledge work with AI assistance. Basic familiarity with using the command line and Python is helpful.

### Instructor
**Jack Wotherspoon**  
Senior Developer Advocate at Google  
[LinkedIn](https://www.linkedin.com/in/jack-wotherspoon/) | [X (Twitter)](https://x.com/JackWoth98)

---

## Course Outline
* Introduction 
* What is Gemini CLI? 
* A Tour of Gemini CLI
* Context is Key: GEMINI.md
* Workflows with Model Context protocol (MCP)
* Customization with Gemini CLI Extensions 
* Gemini CLI for Software Development 
    * Github actions automation 
    * PR review/shell-github 
* Gemini CLI for Data Analysis 
    * Structured data
    * Unstructured data 
    * System logs
    * Source code
    * Visual Data
    * Web Content
    * Communication data (email, chat)
    * Calendar Data
* Gemini CLI for Content Creation
    * NanoBanana extension for image generation 
    * Social media posts/ excerpts from video 
    * Transcript the video 
* Gemini CLI for Learning 
    * Study Guides
    * Practice tests
    * Personal tutor
    * Summarize content 
    * Proof reading 
    * Brain storming 
    * Search grounding 
    * Job search 
* Conclusion 
* Course materials and Installation guide 

---

## Course Materials & Gemini CLI Installation Guide

### Course Materials
Great work completing this course! You can access a repo with all course materials here. Feel free to reuse any prompts and remix and code used in this course!

**Repo Structure**
* `starter_files/` - Initial starter files as they would exist at the start of the course, before any changes have been made.
* `final_files/` - Completed final files as they would exist at the end of the course, after all changes have been made.
* `prompts/` - Prompt templates and files from each lesson, plus bonus tips and commands.

---

## Installation Guide
This guide explains how to install and configure the official Google Gemini CLI (`@google/gemini-cli`).

### Prerequisites
Before installing, ensure your system meets the following requirements:
* **Node.js:** Version 20.0.0 or higher is recommended (Minimum v18).
    * Check version: `node -v`
    * Download: [nodejs.org](https://nodejs.org)
* **Google Account:** Required for authentication (Free tier available).

### Installation Methods

#### Option 1: NPM (Recommended)
This is the standard method for most users (Windows, macOS, Linux). It installs the CLI globally on your system.
1. Open your terminal or command prompt.
2. Run the install command:
   ```bash
   npm install -g @google/gemini-cli
   ```
   *(Note: On Linux or macOS, you might need to use `sudo` if you encounter permission errors: `sudo npm install -g @google/gemini-cli`)*

#### Option 2: Homebrew (macOS)
If you use Homebrew on macOS, you can install it directly.
1. Run the brew install command:
   ```bash
   brew install gemini-cli
   ```

#### Option 3: NPX (No Install / One-time Use)
If you want to run the CLI without permanently installing it, use npx. This always fetches the latest version.
1. Run the command:
   ```bash
   npx @google/gemini-cli
   ```

### Authentication
Once installed, you need to authenticate. The CLI supports a browser-based login flow which is the easiest to set up.
1. Run the CLI for the first time:
   ```bash
   gemini
   ```
2. The CLI will prompt you to select an authentication method.
3. Select **"Login with Google"** (using arrow keys and Enter).
4. A browser window will open. Sign in with your Google Account.
5. Once authorized, close the browser window. The terminal will confirm you are logged in.

#### Alternative: API Key
If you prefer using an API key (e.g., for automated scripts or enterprise environments), you can set it as an environment variable.
1. Get a key from Google AI Studio.
2. Set the variable in your terminal:
    * **Mac/Linux:** `export GEMINI_API_KEY="YOUR_KEY_HERE"`
    * **Windows (PowerShell):** `$env:GEMINI_API_KEY="YOUR_KEY_HERE"`

### Verification
To verify the installation was successful, check the version or run a simple prompt.
```bash
gemini --version
```

[Github repo link](https://github.com/https-deeplearning-ai/sc-gemini-cli-files)
