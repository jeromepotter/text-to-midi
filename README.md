#  Text-to-MIDI Generator

> **A browser-based, generative MIDI interface powered by Gemini 3 Flash that turns natural language into raw note data for your DAW or Hardware Synths.**

## The Vision
Most AI music tools generate audio files (.wav). They are "jukeboxes"—you consume what they give you.

**This tool is an instrument.** It generates **MIDI**, the source code of music.
* **Zero Audio Bloat:** It outputs pure data. You own the sound design.
* **Hardware Ready:** Connect your Prophet, Moog, or Juno via USB and watch the AI play your analog gear in real-time.
* **Infinite Ideation:** Use the AI to break writer's block, generate complex polyrhythms, or create "impossible" piano runs that no human hand could play.

##  Features
* **Powered by Gemini 3 Flash:** Leverages Google's latest model for "High Reasoning" musical composition.
* **Stateful Memory:** The AI remembers your session. You can say *"Make the drums more aggressive"* or *"Change the key to F# Minor"* and it will iterate on the previous idea.
* **Web MIDI API:** Runs entirely in the browser. No Python scripts, no node servers, no installation required.
* **Multi-Channel Support:** Generates independent tracks for up to 16 MIDI channels simultaneously.
* **JSON-to-MIDI Bridge:** Converts the LLM's structured JSON output into millisecond-accurate MIDI events.

##  Setup & Usage

### 1. Prerequisites
You do not need to install software, but you need to route the MIDI data.
* **Mac Users:** Enable the **IAC Driver** in "Audio MIDI Setup."
* **Windows Users:** Install **LoopMIDI** (free) to create a virtual MIDI port.
* **Hardware Users:** Just plug in your USB MIDI Interface.

### 2. Running the App
1.  Download `index.html` from this repository or fo to (https://text-to-midi.netlify.app/)
2.  Open it in Google Chrome, Edge, or Brave (Safari has limited Web MIDI support).
3.  Get a free API Key from [Google AI Studio](https://aistudio.google.com/app/apikey).
4.  Select your **MIDI Output** from the dropdown menu in the app.

### 3. Your First Prompt
Type a prompt that describes the instrumentation, theory, and vibe:
> *"Create a complex Bebop Jazz piece. 220 BPM. Swing feel. Ch 1 (Piano): Sparse, rootless 'Bill Evans' style voicings. Syncopated comping. Ch 2 (Double Bass): Fast walking bass line with triplet skips. Ch 3 (Trumpet): A virtuosic, breathless solo. Use the 'Coltrane Matrix' and chromatic runs. Humanize the velocity and timing significantly."*

##  "Virtuoso" Prompting Strategy
This tool works best when you treat the AI as a session musician who knows music theory but needs direction.

* **Be Specific with Channels:** Map your DAW tracks first. (e.g., "Ch 1 = Bass, Ch 2 = Pad").
* **Use Mathematical Concepts:** The AI excels at logic.
    * *Try:* "Play a Fibonacci sequence rhythm."
    * *Try:* "Create a polymeter where Ch 1 is in 4/4 and Ch 2 is in 5/4."
* **The "Impossible" Hand:** Ask for things humans can't do.
    * *Try:* "Play a 12-note chord spread across 5 octaves that rises and falls like a wave every 3 seconds."

##  Important Notes
* **Browser Support:** Must use a Chromium-based browser (Chrome/Edge) for Web MIDI support.
* **Context Window:** The chat has a memory. If the music gets weird/bad, click **[ CLEAR MEMORY ]** to reset the AI's brain.
* **Hallucinations:** Sometimes the AI might drift off-tempo in long generations (>60s). It is best used for loops and 8-16 bar phrases.

##  Contributing
Feel free to fork this project. Ideas for future updates:
* Standard MIDI File (.mid) download button.
* Visual Piano Roll.
* CC Control (Mod Wheel/Filter) integration.

##  License
MIT License. Go make some noise.
