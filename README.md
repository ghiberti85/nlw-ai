<div align="center">
    <h1>upload.ai</h1>
</div>
</br>
<div align="center">

[**About**](#-about) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Objective**](#-objective) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Features**](#-features) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Demo**](#-demo) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Technologies and Tools**](#-technologies-and-tools) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Project Organization**](#-project-organization) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**Installation and Execution**](#-installation-and-execution) &nbsp;&nbsp;**|**&nbsp;&nbsp;
[**How to Contribute**](#-how-to-contribute) &nbsp;&nbsp;**|**&nbsp;&nbsp;

</div>

## 📃 About

<img alt="upload.ai" src="/upload-ai-web/public/screenshot.png" width="100%"/>

**Upload.ai** is the project developed during the Mastery track of **Next Level Week AI**, an online event produced by [**Rocketseat**](https://github.com/Rocketseat).

It's an application that allows uploading videos and, through AI, automatically generates catchy titles and descriptions with good indexing.

## 🎯 Objective

The central objective of **Upload.ai** is to create a platform that allows users to upload videos and, through **AI** (Artificial Intelligence), automatically generate catchy titles and optimized descriptions for these videos. This application aims to simplify the process of creating video content and improve the visibility of videos on the web.

The **Upload.ai** project has many practical applications. It can help content creators, marketing professionals, online educators, and media companies improve the visibility and performance of online videos, saving time in creating attractive and search engine optimized titles and descriptions.

## ✨ Features

- [x] Video uploading;
- [x] Video to audio conversion using [**ffmpeg.wasm**](https://ffmpegwasm.netlify.app/);
- [x] Audio transcription using [**Whisper (ASR - Automatic Speech Recognition)**](https://openai.com/research/whisper) from OpenAI;
- [x] Customization of prompts;
- [x] Summary generation of transcription using OpenAI's GPT-3 model;
- [x] Generation of catchy titles using OpenAI's GPT-3 model;
- [x] Generation of SEO-optimized descriptions using OpenAI's GPT-3 model;
- [x] Flexibility to set the temperature (level of randomness) of the generated results (0-1);
- [x] Copy of the AI-generated results to the clipboard.

## 💻 Demo

https://github.com/ghiberti85/nlw-ai/upload-ai-web/public/upload-ai-demo.mp4

## 🚀 Technologies and Tools

<table>
  <tbody>
    <tr>
      <td style="font-weight: bold">Front-end (web)</td>
      <td>
        <a href="https://reactjs.org/" target="_blank" rel="noopener noreferrer">React</a>,
        <a href="https://www.typescriptlang.org/" target="_blank" rel="noopener noreferrer">TypeScript</a>,
        <a href="https://tailwindcss.com/" target="_blank" rel="noopener noreferrer">TailwindCSS</a>,
        <a href="https://vitejs.dev/" target="_blank" rel="noopener noreferrer">Vite.js</a>,
        <a href="https://radix-ui.com/" target="_blank" rel="noopener noreferrer">Radix UI</a>,
        <a href="https://ui.shadcn.com/" target="_blank" rel="noopener noreferrer">Shadcn/ui</a>,
        <a href="https://ffmpegwasm.netlify.app/" target="_blank" rel="noopener noreferrer">ffmpeg.wasm</a>,
        <a href="https://axios-http.com/" target="_blank" rel="noopener noreferrer">Axios</a>,
        <a href="https://www.npmjs.com/package/ai" target="_blank" rel="noopener noreferrer">Vercel AI SDK</a>
      </td>
    </tr>
    <tr>
      <td style="font-weight: bold">Back-end (API)</td>
      <td>
        <a href="https://nodejs.org/en/" target="_blank" rel="noopener noreferrer">Node.js</a>,
        <a href="https://www.typescriptlang.org/" target="_blank" rel="noopener noreferrer">TypeScript</a>,
        <a href="https://www.prisma.io/" target="_blank" rel="noopener noreferrer">Prisma</a>,
        <a href="https://www.fastify.io/" target="_blank" rel="noopener noreferrer">Fastify</a>,
        <a href="https://zod.dev/" target="_blank" rel="noopener noreferrer">Zod</a>,
        <a href="https://www.sqlite.org/index.html" target="_blank" rel="noopener noreferrer">SQLite</a>,
        <a href="https://www.npmjs.com/package/openai" target="_blank" rel="noopener noreferrer">OpenAI Node API</a>,
        <a href="https://www.npmjs.com/package/ai" target="_blank" rel="noopener noreferrer">Vercel AI SDK</a>
      </td>
    </tr>
  </tbody>
</table>

## 📂 Project Organization

This repository is divided into two main directories:

- **api**: Contains the back-end source code.
- **web**: Contains the front-end source code.

## 🔧 Installation and Execution

To download the project source code to your machine, you'll first need to have [**Git**](https://git-scm.com/) installed. With Git installed, in your terminal, execute the following command:

```bash
git clone https://github.com/ghiberti85/nlw-ai.git
```

To install dependencies and run the project, you'll need to have [**node.js**](https://nodejs.org/en/) installed on your machine, which comes with npm.

> In this project [**pnpm**](https://pnpm.io/) was used, which aims to save disk space and speed up package installation due to its shared dependency storage approach.

### Front-end (Web)

Navigate to the project folder:

```bash
cd web
```

Install dependencies using **pnpm** or **npm**:

```bash
# pnpm
pnpm install

# npm
npm install
```

Run the project:


```bash
# pnpm
pnpm run dev

# npm
npm run dev
```

The application will be available at http://localhost:5173. You can access it from your browser.

### Back-end (API)

Navigate to the project folder:

```bash
cd api
```

Install dependencies using **pnpm** or **npm**:

```bash
# pnpm
pnpm install

# npm
npm install
```

Create the .env file with the necessary environment variables:

```bash
DATABASE_URL="file:./dev.db"
OPENAI_KEY="sua OpenAI key"
```

Run the following command to generate the Prisma client:

```bash
# pnpm
pnpm prisma generate

# npm
npm prisma generate
```

Execute the database migrations:

```bash
# pnpm
pnpm prisma migrate dev

# npm
npm prisma migrate dev
```

Run the project:

```bash
# pnpm
pnpm run dev

# npm
npm run dev
```

The server will be available at http://localhost:3333.

## 💡 How to Contribute

- **_Fork_** this repository;
- Create a **branch** for your feature: `git checkout -b my-feature`;
- **Commit** your changes: git commit -m 'feat: My new feature';
- **Push** to your branch: git push origin my-feature;
- Create a **pull request** with your feature;

Pull requests are always welcome. If you have questions or suggestions, create an **issue** or contact me.

---

Developed with 💚 by <a href="https://github.com/ghiberti85/">ghiberti85</a>

<div style="display: flex;">
  <a href="https://www.linkedin.com/in/fernando-ghiberti" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" style="margin-right: 2vw" target="_blank"></a>
  <a href="mailto:ghiberti85@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" style="margin-right: 2vw"/></a>
</div>



