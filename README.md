# Nano Banana — AI-Illustrated EPUB Reader

A single-file HTML app that lets you read any EPUB book with AI-generated illustrations that appear in a side panel as you read.

Inspired by [@mrnugget's Moby Dick](https://github.com/mrnugget/moby-dick), but generalized to work with any EPUB file.

## How It Works

1. Open `index.html` in your browser
2. Drop an EPUB file (or click to browse), or paste a blog post/tweet URL
3. Enter your [OpenRouter API key](https://openrouter.ai/keys) when prompted
4. Read — click "Generate Illustration" to illustrate the current chapter, or select specific text to illustrate

## Features

- **EPUB parsing** — Handles EPUB 2/3, TOC navigation, embedded images
- **URL loading** — Pulls readable text from blog posts or tweets for illustration
- **Model selection** — Choose between Nano Banana Flash (~$0.04/img) and Nano Banana Pro (~$0.13/img) via OpenRouter
- **16 illustration styles** — Technical styles (architecture diagram, whiteboard sketch, infographic, concept map, blueprint, engineer's notebook, textbook figure, chalkboard) and fiction styles (Renaissance engraving, watercolor, manga, pencil sketch, Japanese woodblock, comic, oil painting, pixel art)
- **Smart prompting** — Technical styles generate labeled diagrams and visual explanations; fiction styles generate atmospheric artwork
- **Dark mode** — System-aware with manual toggle
- **Image caching** — Previously generated illustrations are cached in memory
- **Request management** — Abort on re-generate, per-model+style+chapter caching
- **Zero dependencies** — Single HTML file, loads JSZip and DOMPurify from CDN

## Requirements

- A modern browser
- An [OpenRouter API key](https://openrouter.ai/keys) (free credits available for new accounts)
