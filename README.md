<div align="center">

# ⚡ StudySpark AI

**Turn any lecture notes into a complete study kit in about 10 seconds.**

Summary · Key terms · Exam tips · Flashcards · Auto-graded quiz · AI tutor chat, in **English or Bangla**.

[![Live Demo](https://img.shields.io/badge/Live_Demo-Open_App-5b4bff?style=for-the-badge&logo=githubpages&logoColor=white)](https://aivietnam-aio-felixdoit.github.io/studyspark-ai/)
[![Offline Demo](https://img.shields.io/badge/Offline_Demo-No_AI_needed-ff7a59?style=for-the-badge)](https://aivietnam-aio-felixdoit.github.io/studyspark-ai/?demo)
[![Pitch Deck](https://img.shields.io/badge/Pitch_Deck-5_slides-1b1f2a?style=for-the-badge)](https://aivietnam-aio-felixdoit.github.io/studyspark-ai/deck.html)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![AI](https://img.shields.io/badge/AI-GPT--4o--mini_via_Puter.js-412991?logo=openai&logoColor=white)
![Hosting](https://img.shields.io/badge/Hosted_on-GitHub_Pages-222?logo=github)
![No API key](https://img.shields.io/badge/API_key-not_required-12a150)
![Hackathon](https://img.shields.io/badge/YUNet_AIgnite_Buildathon-2026-5b4bff)

<img src="docs/screenshots/home.png" alt="StudySpark AI home page" width="850">

</div>

## The problem

Students preparing for SSC, HSC and university exams study from long notes, PDFs and guidebooks. Turning those into summaries, flashcards and practice questions by hand takes hours, so most students just re-read, which is the least effective way to study. Private tutors are expensive and not available at midnight before an exam.

## The solution

Paste your notes (or upload a `.txt`), pick your level and language, and click **Generate**. StudySpark AI reads only your notes and builds:

| Feature | What you get |
|---|---|
| 📝 **Smart summary** | 5–7 key ideas, key terms with meanings, exam tips |
| 🃏 **Flashcards** | 8 tap-to-flip cards with shuffle, for active recall |
| ✅ **Auto quiz** | 5 MCQs with instant feedback, explanations, score and retake |
| 💬 **Ask AI** | A tutor chat that answers from your own notes |
| ⬇️ **Export** | Download the full kit as Markdown, or copy the summary |
| 💾 **Auto-save** | Your last study kit is restored when you come back |

## Screenshots

| Summary | Flashcards |
|---|---|
| <img src="docs/screenshots/summary.png" width="420"> | <img src="docs/screenshots/flashcard-front.png" width="420"><br><img src="docs/screenshots/flashcard-back.png" width="420"> |

| Quiz with instant feedback | Mobile |
|---|---|
| <img src="docs/screenshots/quiz.png" width="420"> | <img src="docs/screenshots/mobile.png" width="260"> |

> Screenshots were taken in demo mode (`?demo`), which loads a pre-built study kit for the bundled sample notes.

## How it works

```
Notes ──▶ Structured prompt (level + language, grounded in notes only)
      ──▶ GPT-4o-mini via Puter.js
      ──▶ JSON {title, summary, keyTerms, examTips, flashcards, quiz}
      ──▶ Validate (retry once if invalid) ──▶ Interactive UI
```

- **No backend, no API key.** AI calls go straight from the browser through [Puter.js](https://puter.com), so the app is free to host and free to use. The first request may show a Puter sign-in popup.
- **Resilient demo.** If the AI service can't be reached while using the sample notes, the app falls back to a pre-built kit, so the product can always be shown.
- **Safe rendering.** All AI output is HTML-escaped before it is shown.

## Run locally

No build step. Clone the repo and open `index.html` in a browser:

```bash
git clone https://github.com/AIVIETNAM-AIO-felixdoit/studyspark-ai.git
cd studyspark-ai
start index.html   # Windows (macOS: open index.html)
```

## Project structure

```
index.html            # The whole app (UI + logic)
deck.html             # 5-slide pitch deck (print to PDF from the browser)
VIDEO_SCRIPT.md       # 2-minute English demo script
docs/screenshots/     # README images
```

## Roadmap

- PDF and photo upload (OCR for handwritten notes)
- Spaced-repetition reminders and progress tracking
- NCTB syllabus-aligned question banks

---

<div align="center">Built for <b>Ostad Presents YUNet AIgnite Buildathon 2026</b></div>
