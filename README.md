# GitHub Pages upload package for REDCap audio survey

This package helps you publish your audio files on GitHub Pages and provides a REDCap instrument CSV that references those files.

## Steps to publish audio on GitHub Pages

1. Create a new GitHub repository (e.g., `redcap-audio`) under your GitHub account.
2. Upload the **contents of this ZIP** into the repository root. Keep the `audio/` folder as-is.
   - You can upload using the GitHub web UI (Add file → Upload files) or git CLI.
3. In the repository, go to **Settings → Pages** (or **Settings → Code and automation → Pages**).
4. Select **Branch: main** (or `master`) and **Folder: / (root)**, then click **Save**. GitHub will publish at:
   `https://<YOUR_GITHUB_USERNAME>.github.io/<REPO_NAME>/`
5. Wait a minute for the site to build. Then confirm one audio file plays by visiting for example:
   `https://<YOUR_GITHUB_USERNAME>.github.io/<REPO_NAME>/audio/a_w3_chong2yang2jie2.wav`
6. Once confirmed, replace `<YOUR_GITHUB_USERNAME>` and `<REPO_NAME>` placeholders in `instrument_github.csv` with your actual username and repo name. Save the CSV.
7. Upload the final `instrument_github.csv` to REDCap **Online Designer → Upload instrument**.
8. Test the survey link — audio should stream inline for participants.

## Notes
- If GitHub Pages uses HTTPS (default), the audio will stream securely and work in REDCap surveys.
- Filenames in `audio/` are preserved; the instrument references them exactly.
- If you want, tell me your GitHub username and repository name and I will generate a final `instrument.csv` with the exact URLs for you.

