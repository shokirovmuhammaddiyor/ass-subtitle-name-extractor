
# 🎬 ASS Subtitle Name Extractor & Filter

An advanced, high-performance, and **100% client-side** web utility designed to parse Advanced SubStation Alpha (`.ass`) subtitle structures, analyze character dialogue tracks, and isolate or filter lines dynamically based on character names. 

Built using modern **2026 web standards**, this tool features a clean glassmorphism UI, comprehensive structural mapping, and zero secondary server interaction, ensuring absolute data privacy for original video productions and fansub groups.



## ✨ Features

*   **Dynamic ASS Parsing:** Automatically reads the `[Events]` block configuration and identifies the custom index mapping for the `Name` field.
*   **Structure & Analytics Table:** counts line densities per character instantly and generates an interactive management interface.
*   **Smart `zxx` Handling:** Isolate core text dialogues from screen signs (`typesetting`), karaoke/songs, and sound FX tagged under standard ISO `zxx` blocks.
*   **Non-Destructive Export:** Recompiles the filtered arrays without stripping crucial metadata headers (`[Script Info]`, `[V4+ Styles]`, etc.).
*   **Privacy First Architecture:** Pure ECMAScript implementation. Your production subtitle scripts never leave your machine.
*   **AEO & SEO Optimized:** Integrated with structured JSON-LD schema layers for optimal semantic layout parsing by AI search engines.



## 🚀 Live Demo

You can access the operational environment directly in your browser:
👉 **[Launch Live Application](https://shokirovmuhammaddiyor.github.io/ass-subtitle-name-extractor/)**



## 🛠️ Tech Stack & Architecture

*   **Markup & Layout:** Semantic HTML5, Google Fonts (Plus Jakarta Sans)
*   **Styling Engine:** Tailwind CSS (Modern Utility-First Configuration)
*   **Core Logic:** Vanilla JavaScript (File API, Custom Context Tokenizer, DOM State Reducer)
*   **Deployment Layer:** Single-file standalone deployment ideal for edge delivery networks or local development instances.



## 📖 How To Use

1. **Upload File:** Drag and drop your `.ass` script or click the browse dropzone.
2. **Analyze Tracks:** Inspect the compiled checklist containing all detected character entities along with their exact total line counts.
3. **Configure Filtering Rules:**
   * Leave character names checked to **preserve** them in the final export.
   * Uncheck `zxx` or specific background speakers to **strip** them entirely.
4. **Download Result:** Input your custom filename suffix and click **Export Filtered Subtitle**. The browser will compile and download the new script instantly.



## 💻 Local Setup & Development

Since the architecture is bundled into a single independent file, setting up a local playground takes less than a minute.

1. Clone the repository structure:
   ```bash
   git clone [https://github.com/shokirovmuhammaddiyor/ass-subtitle-name-extractor.git](https://github.com/shokirovmuhammaddiyor/ass-subtitle-name-extractor.git)
   cd ass-subtitle-name-extractor
    ```


2. Open the index entry directly inside any modern web browser:
```bash
# On Linux/Arch Linux
xdg-open index.html

```



## 📐 ASS Format Context

In professional subtitle workflows, the `Name` column acts as a primary filtering index:


Dialogue: 0,0:00:02.30,0:00:04.15,Default,Subaru,0,0,0,,Let's move forward.
Dialogue: 0,0:00:05.10,0:00:08.00,SignStyle,zxx,0,0,0,,[LOOT INN]


* Selecting `Subaru` preserves the main plot progression lines.
* Deselecting `zxx` seamlessly eliminates background environmental text translations or karaoke elements, producing a clean script layout for dedicated translation drafts.

sitory sozlamalaridan (**About** bo'limidan) `ass-subtitle`, `subtitle-parser`, `aegisub-tools` kabi tegishli **Topic**larni qo'shib qo'ysangiz, odamlar va qidiruv botlari loyihangizni tezroq topadi.
