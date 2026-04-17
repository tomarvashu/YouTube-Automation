# YouTube Automation

An automated YouTube publishing workflow built in n8n. The system reads pending video entries from Google Sheets, generates a YouTube description and hashtags using AI, downloads the selected video from Google Drive, uploads it to YouTube, and updates the publishing status automatically.

## My Role
I initiated this project and defined the workflow structure, publishing logic, and practical use case it was designed to support.

As my role later expanded into broader Operations & Technology leadership, my contribution shifted more toward workflow direction, testing, refinement, and execution oversight. Development was carried forward with support from my internal team, while I remained involved in shaping the system logic, usability, and practical execution flow.

## What It Does
- Reads pending video rows from Google Sheets
- Picks the next pending entry in sequence
- Generates a YouTube description and hashtags using AI
- Prepares structured upload data
- Downloads the video file from Google Drive
- Uploads the video to YouTube
- Updates the source row status to `Completed`

## Workflow Overview
1. A schedule trigger starts the workflow automatically
2. Google Sheets is read for rows marked `Pending`
3. The next pending row is selected
4. AI generates the description and hashtags
5. Upload metadata is prepared
6. The video file is downloaded from Google Drive
7. The video is uploaded to YouTube
8. The sheet row is updated to `Completed`

## Tech Stack
- n8n
- Google Sheets
- Google Drive
- YouTube API
- OpenAI
- JavaScript

## Use Case
This workflow is useful for teams that want to streamline YouTube publishing by combining structured content planning, AI-generated metadata, and automated upload execution.

## Notes
Before using this workflow publicly, remove or replace:
- private sheet IDs
- internal file IDs
- account credentials
- company-specific prompts or naming conventions
