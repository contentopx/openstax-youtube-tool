# 📹 OpenStax YouTube Uploader

This script automates the process of uploading educational videos (e.g., from OpenStax) to YouTube using the YouTube Data API. It also updates a CSV log with the video status and mapping information.

## 🔧 Features

- Authenticates with Google OAuth to access your YouTube channel
- Uploads videos from a CSV list
- Automatically creates or matches to a YouTube playlist
- Downloads video files from OpenStax URLs
- Updates and saves new CSV files with YouTube video links and status

📄 CSV Format
Your input CSV should contain at least these columns:

Descriptive content title

Description

link to video source

Playlist (can be blank — auto-filled)

YouTube URL (will be updated)

DescriptionWithTags (auto-filled if empty)

✅ Output
K12_YouTube_Upload_Updated.csv: includes upload status and YouTube URLs

videomapping.csv: simplified reference of source → YouTube mapping

🛑 Notes
Vimeo-hosted videos are skipped unless authorized tokens are available

Broken or failed video links are logged and marked accordingly

Only public playlists are supported

Upload quota or API errors are handled gracefully with messages

