# AI Video Production Studio

A personal, self-hosted tool that automates end-to-end YouTube video production for
a single creator's own channel: script generation, text-to-speech narration, audio
mixing, video rendering, thumbnail creation, and — optionally — uploading the
finished video to the operator's own YouTube channel.

This repository exists solely to provide the public homepage and privacy policy
required for YouTube Data API review. The application itself is source-available
only to its operator; this page documents its behavior for reviewers and users.

- **Homepage:** https://ricardoschroeder.github.io/video-studio-info/
- **Privacy Policy:** https://ricardoschroeder.github.io/video-studio-info/privacy.html

## What it does

The tool runs locally on the operator's own machine. Given a topic, it generates a
video script with an LLM, narrates it with text-to-speech, mixes narration with
background music, renders the final video, generates a thumbnail, and writes
YouTube metadata (title, description, tags). The operator reviews the result and
can choose to upload it to their own YouTube channel directly from the tool.

## YouTube API usage

The tool uses the YouTube Data API v3 to act on the operator's own channel only:

- `youtube.channels.list` — to confirm which channel is connected.
- `youtube.videos.insert` — to upload a finished video produced by the operator.
- `youtube.thumbnails.set` — to set a custom thumbnail on that upload.

There is no other user-facing surface. It is not distributed to or used by anyone
other than its operator.

## Data handling

See the [Privacy Policy](https://ricardoschroeder.github.io/video-studio-info/privacy.html)
for full details on how OAuth credentials are stored and how access can be revoked.
