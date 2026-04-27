# Chooser

Chooser helps you compare several audio takes without being swayed by filenames or upload order. It plays two takes at a time, asks which one you prefer, and builds a ranking from your choices.

Use it when you have a few reads of the same line and want a clear winner.

## Quick Start

1. Enter a user key you will recognise later.
2. Upload your audio files, or upload a ZIP containing the files.
3. Choose the line or group you want to compare.
4. Listen to A and B.
5. Click `Prefer A` or `Prefer B`.
6. Keep going until the ranking is complete.
7. Download the JSON progress backup before you close the page.

## Naming Your Files

The cleanest filename format is:

```text
LineKey.takeNumber.ext
```

Example:

```text
Line1.6.mp3
```

That tells Chooser that this is take 6 for `Line1`.

Supported audio formats include MP3, WAV, M4A, AAC, OGG, and FLAC, although browser playback can vary by device.

If the filenames do not match the expected format, Chooser will put all uploaded files into one blind comparison group. That is fine if you simply want to compare a loose batch of takes.

## Uploading A ZIP

ZIP uploads are useful when you have lots of files.

Before uploading:

- Put only the audio takes you want to compare in the ZIP.
- Avoid nested folders if you can.
- Use the same `LineKey.takeNumber.ext` pattern where possible.

If the ZIP is too large, contains too many files, or contains no supported audio, Chooser will stop and show an error instead of trying to process it badly.

## Saving And Restoring Progress

Chooser can briefly remember progress for the same user key, but you should not rely on that as your only backup.

The safer habit is:

1. Download `Download all progress (JSON)` whenever you have made useful progress.
2. Keep the original audio files as well.
3. To restore later, upload the JSON backup first, then upload the matching audio files again.

The JSON backup stores your comparison results and rankings. It does not contain the audio itself.

## Deleting Bad Takes

Use `Delete A` or `Delete B` when a take is unusable and should be removed from that line's comparison.

This affects the current Chooser session and progress backup. It does not delete the original file from your computer.

## What You Get

Chooser gives you:

- an on-screen ranking for each line or group
- tie-break ranking where needed
- a JSON backup of all comparison progress

## If Something Looks Wrong

- If everything appears as one group, check the filenames.
- If restored progress appears but audio does not play, upload the matching audio files again.
- If the browser will not play a file, try MP3 or WAV.
- If you are unsure whether progress is safe, download the JSON backup immediately.

## What Chooser Is Not

Chooser is not an audio editor. It does not change, trim, clean, or export audio. It only helps you choose between takes.
