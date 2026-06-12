# Production Log

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
