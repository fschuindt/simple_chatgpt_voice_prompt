# Simple ChatGPT Voice Prompt

A simple example on how to use 3rd party APIs to prompt ChatGPT with voice. Responses will also be given in generative AI voice by Elevenlabs.

Currently, context is being dropped every new prompt.

It uses the following web APIs:
- OpenAI Whisper
- OpenAI ChatGPT
- [Elevenlabs.io](https://elevenlabs.io/)

## Installation

Install the following dependencies.

- [parecord](https://command-not-found.com/parecord)
- [FFmpeg](https://ffmpeg.org/)
- [Whisper CLI](https://github.com/vatsalaggarwal/whisper-cli)
- [SGPT](https://github.com/tbckr/sgpt)
- [curl](https://curl.se/)

For Whisper CLI and SGPT, make sure you have also configured their respective API keys.

For the Elevenlabs API key, just export it like so:
```
export ELEVENLABS_API_KEY=your_key_here
```
## Usage

```
./simple_chatgpt_voice_prompt
```

Start speaking, then enter `Ctrl + C` when done recording your message. Wait for the voice response.

All audio files are kept within the `./recordings` folder. `.wav` files are the original prompt, `.mp3` files are the original prompt converted into MP3 for lower file sizes and, `.mpeg` files are the generative voice responses.
