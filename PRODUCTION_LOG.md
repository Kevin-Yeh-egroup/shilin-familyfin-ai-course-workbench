# Production Log

## 2026-06-12 Update 4

- Follow-up: clarified that 時間資源盤點 can help identify where 用藥追蹤 and 服務追蹤 might connect to future workflow design, while not presenting medication reminders, service tracking, or automatic notifications as current tool features.
- Revised the course outline after Kevin's clarification:
  - Day 1 keeps 手機錄音、語音轉文字、個案歷程紀要、時間資源盤點、知識庫 / 問問 AI / 社工儀表板.
  - Day 2 now focuses on 既有自我檢測, 自我檢測結果讀法, 心理相關自我檢測共創可能, and resource connection.
- Removed the unused quick-screen course segment from the page, copy output, Markdown outline, and Word download because it is not part of this course version.
- Revised 時間資源盤點 wording to only describe confirmed behavior from the referenced tool: 新增一段時間, 日期/時段, 活動內容, 今日 24 小時盤點, 已記錄時數, 可補充時間, 最近紀錄.
- Regenerated `shilin-familyfin-two-day-course-outline-v0.1.docx`; structural DOCX check passed with 2 tables, row counts `[7, 8]`.
- Render-to-PNG visual QA still could not run because LibreOffice/soffice is unavailable in this environment; structural DOCX checks were used instead.
- Local human-like check passed on the packaged HTML: curriculum section showed the revised self-check course, copy button showed success, Word file existed, and mobile viewport had no horizontal overflow.
- Search posture preserved: HTML meta robots, `robots.txt`, and Vercel `X-Robots-Tag` should remain noindex for review-stage sharing.

## 2026-06-12 Update 3

- Added curriculum-section actions in the top-right of `第一版課綱草案`:
  - `複製兩天課綱`
  - `下載 Word`
- Added `shilin-familyfin-two-day-course-outline-v0.1.docx` as the Word download file for the two-session outline.
- The copy/download content is limited to the two-day curriculum: title, course goal, Day 1 schedule, and Day 2 schedule.
- DOCX structural check passed: 2 tables, 7 rows for Day 1 table including header, 8 rows for Day 2 table including header.
- Render-to-PNG visual QA could not run because LibreOffice/soffice was unavailable in this environment; structural DOCX checks were used instead.
- Search posture preserved: HTML meta robots, `robots.txt`, and Vercel `X-Robots-Tag` should remain noindex for review-stage sharing.

## 2026-06-12 Update 2

- Swapped `時間盤點工具` with `知識庫、問問 AI 與社工儀表板` in the two-session outline.
- Promoted the time audit tool into Day 1 and framed it as a core support for 用藥管理 and 服務追蹤管理.
- Moved `知識庫、問問 AI 與社工儀表板` into Day 2 as the resource-search and review-draft step.
- Added mobile recording basics to `語音轉文字`: how to record, how to find the audio file in the phone recording/files app, and how to use only simulated audio for class.
- Reviewed and aligned course axes, tool ranking, safe demos, pre-course materials, traffic-light boundaries, output artifacts, and generated summary copy.
- Search posture preserved: HTML meta robots, `robots.txt`, and Vercel `X-Robots-Tag` should remain noindex for review-stage sharing.

## 2026-06-12 Update

- Removed the course-boundary paragraph Kevin asked to delete from the teaching page.
- Moved `第一版課綱草案` between `課程主軸` and `從需求選工具`.
- Revised the two-session outline:
  - Day 1: 語音轉文字、個案歷程紀要、知識庫、問問 AI 與社工儀表板。
  - Day 2: 個案歷程紀要工作流、時間盤點工具概念、免費財務諮詢、急難專區。
- Synced `course-outline-v0.1.md` with the same two-session structure.
- Added an empty data favicon link to avoid browser `/favicon.ico` 404 noise during QA.
- Search posture preserved: HTML meta robots, `robots.txt`, and Vercel `X-Robots-Tag` should remain noindex for review-stage sharing.

## 2026-06-12

- Artifact: 士林地檢署心理師好理家在 AI 課程工作台
- Package slug: `shilin-familyfin-ai-course-workbench`
- GitHub repo: `https://github.com/Kevin-Yeh-egroup/shilin-familyfin-ai-course-workbench`
- Vercel project: `egroup-task3s-projects/shilin-familyfin-ai-course-workbench`
- Primary public URL: `https://shilin-familyfin-ai-course.vercel.app/`
- Vercel project alias: `https://shilin-familyfin-ai-course-workbenc.vercel.app/`
- Public posture: GitHub public repo + Vercel Production URL
- Search posture: review-stage noindex enabled by HTML meta robots, `robots.txt`, and Vercel `X-Robots-Tag`
- Sensitive data posture: no real case data, no login data, no internal system export
- Deployment protection: project-level `ssoProtection` set to `null` so the public Vercel URL is accessible without Vercel login
- Verification: root URL returned `200 OK`; response header included `X-Robots-Tag: noindex, nofollow, noarchive`; `robots.txt` returned `Disallow: /`; HTML contained the meta robots tag and the expected course sections
