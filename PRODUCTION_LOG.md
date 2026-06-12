# Production Log

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
