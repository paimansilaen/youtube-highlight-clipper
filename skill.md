name: YouTube highlight clipper description: Use when someone gives a YouTube, podcast, X Space or stream link and wants it cut into short highlight clips with burned-in captions, a title, a watermark and an optional AI voice-over.
YouTube highlight clipper
Turn a long video (YouTube, podcast, livestream replay, X Space/broadcast) into short, punchy highlight clips ready to post.

0. Collect the brief (ask only what's missing)
Source link(s) and optional timestamps or a list of "best moments" (e.g. the creator's own review points).
Platform/format: horizontal 1920x1080 (X, YouTube) or vertical 1080x1920 (Reels, Shorts, TikTok).
Watermark/handle text, and an optional avatar/logo image for a corner.
Language for captions and voice-over.
Voice-over: none, or a TTS provider + voice ID. Captions: on or off.
Clip count and target length (default 30–90 s each).
1. Download and inspect

yt-dlp -f "bv*[height<=1080]+ba/b" --merge-output-format mp4 -o source.mp4 "<URL>"
ffprobe -v error -show_entries format=duration -of csv=p=0 source.mp4
If the link is unavailable or members-only, stop and ask for a file upload.
