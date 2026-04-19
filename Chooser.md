# Chooser

Chooser is a Streamlit app for blind audio take comparison.

It is built for situations where you have several takes of the same line and want a structured way to decide which read is strongest without being biased by filenames, order, or memory.

## What It Does

- Upload multiple audio takes directly, or upload a ZIP archive.
- Compare takes blind, two at a time.
- Record the preferred take for each comparison.
- Rank takes per line using comparison results and tie-break logic.
- Delete unusable takes during review.
- Save and restore progress with a user key.
- Export all progress as a JSON backup.

## Upload Formats

Preferred filename format:

```text
LineKey.takeNumber.ext
```

Example:

```text
Line1.6.mp3
```

Supported audio formats include:

- MP3
- WAV
- M4A
- AAC
- OGG
- FLAC

If uploaded files do not use the preferred filename format, Chooser treats the uploaded files as one blind comparison group. This is useful when you simply want to compare a batch of arbitrary takes against each other.

## Basic Workflow

1. Enter a user key.
2. Upload audio files or a ZIP archive.
3. Choose the line/group to compare.
4. Listen to A and B without filename context.
5. Choose the preferred take.
6. Continue until the line is complete, or stop early when a clear leader cannot be overtaken.
7. Download the JSON progress backup when needed.

## Progress

Chooser can restore saved progress for the same user key for a short resume window after use. For longer-term safety, use the JSON download and import tools.

The JSON backup stores comparison progress and ranking data. It does not replace the original audio files; to continue a restored comparison, upload the corresponding audio again.

## Outputs

Chooser provides:

- On-screen ranking per line/group.
- A downloadable JSON file containing all comparison progress.

## Notes And Limitations

- Chooser is a listening and ranking tool, not an audio editor.
- It does not alter the uploaded audio files.
- The quality of the ranking depends on the comparisons made.
- If filenames are inconsistent, Chooser deliberately falls back to treating the upload as a single comparison group.

