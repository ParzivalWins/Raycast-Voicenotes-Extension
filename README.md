# Raycast Voicenotes Extension

Search and filter your [Voicenotes.com](https://voicenotes.com) recordings directly from Raycast.

## Features

- **Search Notes**: Quickly find your voice notes by title or content.
- **Tag Filtering**: Filter your notes by tags (e.g., `#ideas`, `#meeting`).
- **View Transcripts**: Read the full transcript of your notes without leaving Raycast.
- **Quick Actions**:
  - Open note in browser.
  - Copy transcript to clipboard.

## Installation

Install via the [Raycast Store](https://www.raycast.com/store).

## Configuration

The first time you run a command, you will be asked for your **Voicenotes API Token**.
You can find this in your Voicenotes settings under **Integrations > Obsidian**.

## Technologies Used

- [Raycast API](https://developers.raycast.com)
- TypeScript
- React

## Publishing Updates to Raycast

To submit future updates to the official Raycast Store without dealing with their massive monorepo download every time, you can clone your fork using a fast "sparse-checkout":

1. Run this snippet to instantly clone only the `voicenotes` extension from your fork:
   ```bash
   git clone --filter=blob:none --no-checkout -b ext/voicenotes --single-branch https://github.com/ParzivalWins/raycast-extensions.git raycast-update-fast
   cd raycast-update-fast
   git sparse-checkout set extensions/voicenotes
   git checkout
   ```
2. Copy the files from your personal repository over into the `extensions/voicenotes` folder.
3. Commit the changes, push your branch, and PR to the Raycast monorepo!
