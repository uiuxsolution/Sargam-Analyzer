# Sargam Note Analyzer

A Python application that analyzes audio files to detect Sargam notes (Indian classical music notation) and displays them in real-time along with lyrics recognition support for both Hindi and English songs.

## Features

- **Real-time Sargam Note Detection**: Analyzes audio files and identifies Sargam notes (Sa, Re, Ga, Ma, Pa, Dha, Ni)
- **Visual Note Display**: Shows the current note being played with a highlighted visualization
- **Progress Tracking**: Includes a progress bar to track the playback position
- **Lyrics Recognition**: Supports both Hindi and English lyrics detection
- **Interactive Controls**: Play/Stop functionality with a user-friendly interface
- **MP3 File Support**: Compatible with MP3 audio files

## Installation

1. Clone this repository or download the source code
2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

Required dependencies:
- librosa (0.10.1)
- numpy (1.24.3)
- sounddevice
- SpeechRecognition (3.10.0)
- soundfile (0.12.1)

## Usage

1. Run the application:
```bash
python sargam_analyzer.py
```

2. Use the interface:
   - Click "Upload MP3" to select an audio file
   - Wait for the analysis to complete
   - Click "Play" to start playback and note visualization
   - The current note will be highlighted in yellow
   - Lyrics will be displayed in the text area (if detected)
   - Use the Stop button to end playback

## Technical Details

- Uses librosa for audio processing and pitch detection
- Implements Google Speech Recognition for lyrics detection
- Frequency ranges for Sargam notes:
  - Sa: 240-260 Hz (C)
  - Re: 270-290 Hz (D)
  - Ga: 300-320 Hz (E)
  - Ma: 320-340 Hz (F)
  - Pa: 360-380 Hz (G)
  - Dha: 400-420 Hz (A)
  - Ni: 440-460 Hz (B)
  - Sa2: 480-500 Hz (Higher C)

## Note

- For best results, use clear audio recordings
- Lyrics recognition works best with clear vocals
- Supports both Hindi and English lyrics detection automatically

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.