# Google 文件助手

Personal Lark Base extension: upload local files or selected record attachments to Google Drive, optionally convert supported files to Google Workspace formats, and write open links back to the selected record.

This repository contains the static production build. Host the root directory with GitHub Pages and use the resulting HTTPS URL as the Lark custom extension service URL.

Google OAuth uses the limited `drive.file` scope. Configure the Pages origin in the Google OAuth web client. Google access tokens remain in browser memory. An authenticated Supabase backend encrypts long-term Google credentials and renews them automatically. The browser stores a revocable app session; use the extension’s sign-out button to stop automatic connection. Sessions expire after 30 inactive days or a maximum of 180 days. Files are sent directly from the browser to Google Drive; GitHub hosts only the extension assets.

Built with @lark-base-open/js-sdk 1.0.2 (ISC). Bundled third-party notices are retained in app.js.
