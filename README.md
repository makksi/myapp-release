# myapp-release
Collection of python compiled programs for windows

# GV: Graphviz DOT Editor

Un editor per file DOT di Graphviz con anteprima in tempo reale, evidenziazione della sintassi e supporto per più formati di esportazione.

![image](https://github.com/makksi/GraphViz_UI/blob/fa636e282edba0cf6f7a19ce89fa0c99f3ab4c77/assets/preview.jpg))



## Funzionalità

- 🖥️ **Anteprima in tempo reale** del grafico mentre scrivi il codice DOT
- 🌈 **Evidenziazione della sintassi** per il linguaggio DOT
- 📑 **Gestione a schede** per lavorare su più file contemporaneamente
- 🔍 **Zoom e pan** dell'anteprima del grafico
- 📁 **Supporto per i formati** .dot e .gv
- 🖼️ **Esportazione** in PNG, SVG, JPG e altri formati
- ⚙️ **Preferenze configurabili** per personalizzare l'esperienza
- ⌨️ **Scorciatoie da tastiera** per le operazioni comuni


## Licenza

Questo progetto è rilasciato sotto licenza MIT. Vedere il file LICENSE per i dettagli.

## Autore

Massimo Scardaci - massimo.scardaci@gmail.com

## Contributi

I contributi sono benvenuti! Apri una issue o una pull request per suggerire miglioramenti.


# Video Cutter

A simple and powerful video processing tool built with Python and Tkinter that allows you to easily cut video files, extract frames, and create PDFs from extracted frames.

![Video Cutter Screenshot](https://github.com/makksi/Vgui/blob/master/assets/screenshot.jpg)

## Features

- **Cut Video Segments**: Trim videos by specifying start and stop time in HH:MM:SS format
- **Frame Extraction**: Automatically extract key frames from videos based on scene changes
- **PDF Creation**: Generate PDF files from extracted frames
- **User-Friendly Interface**: Simple and intuitive GUI for easy video processing
- **Video Preview**: Open original or processed videos directly from the application

## Requirements
- FFmpeg (external dependency)
- [Optional] jpeg2pdf (for PDF creation)

## Installation

1. Download the latest zip file
2. Download and install [FFmpeg](https://ffmpeg.org/download.html) on your system.
3. [Optional] Download jpeg2pdf if you plan to use the PDF creation feature.

## Usage

1. Run the application:
2. Select a video file using the "Browse" button.
3. Set the FFmpeg executable path (this will be saved for future use).
4. Choose one of the following operations:

   - **Cut Video**:
     - Set the start time and stop time in HH:MM:SS format
     - Click the "CUT" button
     - Once processed, click "Open CUT Video" to view the result

   - **Extract Frames**:
     - Click the "Extract Frames" button
     - Frames will be saved in a subfolder named after the video

   - **Create PDF from Frames**:
     - After extracting frames, click "Create PDF from Frames"
     - The PDF will be saved in the frames directory as "ALL.pdf"

## Configuration

The application saves your FFmpeg executable path in a configuration file (`cut_gui.ini`) in the application directory for convenience.

## How it Works

- Video cutting uses FFmpeg with the `libx264` codec for video and copy mode for audio
- Frame extraction uses FFmpeg's scene detection with a threshold of 0.1
- PDF creation uses the jpeg2pdf utility to combine the extracted frames

## Troubleshooting

- Ensure FFmpeg is properly installed and the path is correctly set
- For PDF creation, make sure jpeg2pdf is available in the same directory as FFmpeg
- If you encounter errors, check that the time format is correct (HH:MM:SS)

## 📄 License

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)]

This project is licensed under the MIT License

## Credits

Massimo Scardaci - massimo.scardaci@gmail.com

---

Feel free to contribute to this project by submitting issues or pull requests!

