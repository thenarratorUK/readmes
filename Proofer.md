# Proofer

Proofer is a Streamlit app for audio proofing.

It lets you upload audio, listen through it, log issues at precise timestamps, and export timestamped notes for use in editing workflows.

## What It Does

- Upload one or more audio files.
- Play audio in the browser.
- Log issues at the current playback time.
- Add labels and notes to each logged issue.
- Review and edit the issue log.
- Export a Reaper marker CSV.
- Export raw log data as CSV.
- Export per-file marker CSVs in a ZIP when multiple audio files are used.

## Supported Audio

Proofer is designed for common browser-playable audio files, including:

- MP3
- WAV

Browser and deployment support may affect which formats can be played.

## Basic Workflow

1. Enter a user key.
2. Upload one or more audio files.
3. Select the active audio file.
4. Play the audio.
5. When you hear an issue, log it with a label and note.
6. Review or edit the logged issues.
7. Download the Reaper CSV or raw log CSV.

## Export Formats

### Reaper CSV

The Reaper CSV is designed for marker-style editing workflows. Each logged issue is exported with timestamp information so it can be brought into Reaper as a practical pickup or proofing reference.

When a single audio file has logged issues, Proofer exports one CSV.

When multiple audio files have logged issues, Proofer exports a ZIP containing one CSV per audio file.

### Raw Log CSV

The raw log CSV includes the detailed app log fields, including audio filename, seconds, timecode, label, note, and logging time.

## Progress

Proofer can restore the log, uploaded audio catalogue, and last-played reminder for the same user key for a short resume window after use.

This is intended for brief interruptions rather than long-term archival storage.

## Privacy Notes

Only upload audio you have the right to process. Proofer is intended as a practical proofing tool, not a permanent storage system.

## Limitations

- Browser playback behaviour can vary by file type and device.
- Exported timestamps depend on the playback time reported by the audio player.
- Proofer does not edit the audio itself; it creates proofing notes and marker exports.

