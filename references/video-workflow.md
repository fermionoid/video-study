# From video to illustrated text

## Open and watch

Use the environment's Computer Use tool with its documented browser or desktop API. Open the supplied replay in the appropriate browser or use the existing player tab. For local media, open it in an available player. Respect any browser or app preference in the request. Use the player's visible controls to identify the duration, caption options, seek position and fullscreen or theater mode. Work in the user's accessible session. If playback requires a sign-in or permission the user needs to provide, continue with any supplied media or captions while reporting the access issue.

Watch the opening and representative moments to establish what is on screen. For a complete illustrated transcript, use the transcript timeline to cover the full requested range and inspect each candidate slide or scene change. For a walkthrough, watch each interaction in sequence so screenshots show both the action and its result when that distinction matters. For illustrated notes, select frames that explain the material. Examples include diagrams in a lecture, a physical object in an interview, a changed setting in a demo, or the visible result of a task in a screen recording. Skip redundant frames.

## Get the words

Prefer the replay's captions or an available transcript export. Keep the original times and language. Use supplied captions or a supported media connector when that makes retrieval easier. If captions are absent or unusable, use the installed media-learning workflow or another authorized transcription method. For local or private recordings, prefer an available local transcription path. A screenshot alone cannot establish spoken words. If no audio or transcript is available, label the output as an account of what is visible and explain the missing speech coverage.

Use captions to choose candidate time windows, then inspect the video around each one. Check that the visible frame actually corresponds to the spoken passage. A speaker can discuss a slide before it appears or after it is gone.

## Capture and align

1. Seek and pause on a stable, sharp frame after any transition. Maximize the video area and allow transient controls to disappear. Prefer the player region if Computer Use supports it. Use the tool's documented screenshot and save/export capabilities.
2. Record the actual player timestamp for the frame, a short description of what is visible, and the matching transcript passage or step. Use the replay's clock even if the deliverable starts later. Visually inspect the image for missing edges, captions covering a diagram, stale frames or unreadable text. Retake nearby if needed.
3. Save images as portable assets and place each beside its matching text. Captions should explain what the image contributes. When a frame shows a different moment from the accompanying quote, preserve both times when that helps the reader find them. If exact alignment is unknown, mark it as approximate or leave the image in a labeled appendix.

If Computer Use can inspect the player but cannot persist a usable image, use an authorized local video copy or a supplied frame. For a local file, FFmpeg can extract a sharp frame from a time identified during review:

```sh
ffmpeg -hide_banner -loglevel error -ss 00:05:23.500 -i recording.mp4 -frames:v 1 frame-00-05-23.500.png
```

Use that same local path when Computer Use is unavailable. If only an inaccessible replay link is available, describe the specific gap and work from any supplied transcript. Never substitute a generated image for a video frame. State what range was covered and whether the images are selected examples or all identifiable slide changes. Export and check the requested deliverable using the main skill.
