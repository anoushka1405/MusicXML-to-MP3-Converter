# MusicXML-to-MP3-Converter

A simple Python GUI tool that converts MusicXML (.mxl) files to MP3 audio files using MuseScore's command-line interface.

---

## Features

- Browse and select `.mxl` MusicXML files easily with a GUI.
- Convert MusicXML files to MP3 format automatically.
- Displays conversion status and error messages.
- Runs conversion in a separate thread to keep the interface responsive.

---

## Prerequisites

- **MuseScore 4** must be installed on your machine.

  - Download from [MuseScore Official Site](https://musescore.org/en/download).
  
- You need to know the path to the MuseScore executable (`mscore` or equivalent).

---

## Setup

1. Clone or download this repository.

2. Ensure you have Python 3 installed.

3. Install required Python modules (if needed):

    ```bash
    pip install tk
    ```

4. Update the MuseScore path in the configuration:

   - Run the script once; it will create a `config.json` file automatically.
   - Open `config.json` and update the `"musescore_path"` value with the correct path to your MuseScore executable.

   Example `config.json`:

   ```json
   {
     "musescore_path": "/Applications/MuseScore 4.app/Contents/MacOS/mscore"
   }
## Usage

1. Run the Python script:

    ```bash
    python musicxml_to_mp3_converter.py
    ```

2. In the GUI window:

    - Click **Browse** to select a `.mxl` MusicXML file.
    - Click **Convert to MP3** to start the conversion.
    - Watch the status label for conversion progress and completion.

3. The output MP3 file will be saved in the same directory as the input `.mxl` file.

---

## Notes

- MuseScore must be installed and accessible at the configured path for conversion to work.
- This tool acts as a GUI wrapper around MuseScore’s conversion command and requires MuseScore installed locally.
- The output MP3 file will be saved in the same directory as the input `.mxl` file.

---

## Limitations & Future Improvements

- Currently requires MuseScore installed on the local machine.
- Could be extended to support other platforms or automate MuseScore installation.
- May add support for other input formats (PDF, MIDI) in the future.
- Add option to customize output directory or filename.

---

## License

MIT License — feel free to use and modify!

