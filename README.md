# American English Speech Dataset

Free sample recordings from Spirelight's off-the-shelf American English speech dataset. 965 hours of unscripted US English conversation recorded in March and April 2026: 1,517 remote conversations between 180 American English speakers, each speaker recorded on their own device and channel, 38 minutes on average. Machine transcripts with speaker labels and word-level timestamps cover every conversation. Download access within 24 hours of a signed order.

**Full dataset, pricing and quotes:** [spirelight.ai/datasets/english-usa](https://www.spirelight.ai/datasets/english-usa?src=github-english-usa)

## Listen

Short excerpts, as played on the dataset page, are in [`excerpts/`](excerpts/):

- [`excerpts/us-english-conversation-excerpt.mp3`](excerpts/us-english-conversation-excerpt.mp3)

The complete sample recordings (FLAC, with transcripts and a `datasets` loader) are on Hugging Face: [huggingface.co/datasets/SpeechDataAI/american-english-speech-dataset](https://huggingface.co/datasets/SpeechDataAI/american-english-speech-dataset). Their uncorrected machine transcripts, as TXT and JSON with word-level timestamps, are also in [`transcripts/`](transcripts/) here.

## Full sample recordings (on Hugging Face)

2 complete recordings, 92 minutes in total. The audio is unedited and compressed losslessly to FLAC on Hugging Face; buyers receive WAV plus one file per speaker for conversations. Each recording has its uncorrected machine transcript as TXT and JSON.

| File | Type | Length | Audio |
| --- | --- | --- | --- |
| [`conversation/american-english-conversation-01.flac`](https://huggingface.co/datasets/SpeechDataAI/american-english-speech-dataset/blob/main/conversation/american-english-conversation-01.flac) | Conversation | 60 min | 48 kHz, 24-bit, stereo |
| [`conversation/american-english-conversation-02.flac`](https://huggingface.co/datasets/SpeechDataAI/american-english-speech-dataset/blob/main/conversation/american-english-conversation-02.flac) | Conversation | 31 min | 48 kHz, 24-bit, stereo |

On Hugging Face, each audio folder has a `metadata.csv` with the full transcript text, so the dataset viewer and `datasets` can read it directly. Word-level timestamps are in the JSON files under `transcripts/`.

```python
from datasets import load_dataset

ds = load_dataset("SpeechDataAI/american-english-speech-dataset", "conversation", split="train")
print(ds[0]["text"][:300])
```

## The full dataset

| Recording type | Recordings | Hours | Average length |
| --- | ---: | ---: | ---: |
| Conversation between two American English speakers | 1,517 | 965.3 | 38 min |

The same collection holds another 236 hours where at least one speaker gives British or another English as their dialect, including 130 hours of American and British speakers talking to each other. Ask if mixed accents suit your project.

- **Speakers:** 180 speakers who give American English as their dialect. Of the 85 who stated a gender, 46 are male, 38 female and 1 non-binary. Of the 108 who stated an age, 17 are 18 to 24, 35 are 25 to 34, 24 are 35 to 44, 16 are 45 to 54 and 16 are 55 or older.
- **Recorded:** 2026-03-02 to 2026-04-03
- **Audio:** 48 kHz, 24-bit WAV recorded with one microphone per speaker. Delivered as a stereo file with one speaker per channel plus one file per speaker.
- **Devices and setting:** 90% recorded on a laptop and 9% on a phone, each speaker on their own device in a quiet environment.
- **Transcripts:** Machine transcripts with speaker labels, segment start and end times and word-level timestamps, as TXT and JSON, for every conversation. Not human-reviewed.
- **Topics:** About 1,000 distinct topic labels chosen by the speakers, most often everyday life, food, history, relationships, music, culture, sports and travel.
- **Licence:** commercial use under a written licence; voice cloning is excluded.
- **Price:** $35 per audio hour for all 965 hours ($33,775); a part of the dataset is quoted.
- **Delivery:** download access within 24 hours of a signed order.

## Good for

- Training and evaluating American English ASR (speech recognition) on unscripted speech rather than read sentences.
- Speaker diarization: in the conversations each speaker has their own channel, so turns and overlaps can be read from the channels.
- Voice agents and turn-taking research: real interruptions, backchannels and topic changes.

Not for voice cloning or imitating a speaker.

## How the samples differ from free corpora

Common Voice and FLEURS are short sentences read aloud, and LibriSpeech is audiobooks read aloud. These recordings are unscripted conversation, 38 minutes per recording on average.

## Licence for this sample

The files in this repository are free to download and use to evaluate whether the full dataset fits your project. Training on them, redistributing them and voice cloning are not permitted. See [LICENSE.md](LICENSE.md). The full dataset is licensed commercially: [request a quote or the full sample pack](https://www.spirelight.ai/datasets/english-usa?src=github-english-usa#request-samples).

## About

Published by SpeechData.ai, part of Spirelight (Spire Light ApS, Denmark), which records, transcribes and licenses speech data for teams building voice AI. Browse every dataset at [spirelight.ai/datasets](https://www.spirelight.ai/datasets?src=github-english-usa).
