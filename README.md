# DataLearn GitHub Pages Website

A ready-to-deploy Jekyll website for DataLearn.

## Deploy

1. Create a GitHub repo named `datalearnvn.github.io`.
2. Upload all files in this folder to the repo root.
3. Go to **Settings → Pages**.
4. Select **Deploy from branch** → `main` → `/root`.
5. Visit `https://datalearnvn.github.io/`.

## Add a daily post

Create a new file in `_posts`:

```text
_posts/YYYY-MM-DD-title.md
```

Example:

```md
---
layout: post
title: "PySpark Lazy Evaluation"
subtitle: "Why Spark waits before executing your code."
date: 2026-05-04
categories: data-science pyspark
image: /assets/images/data-platform.png
---

Your content here.
```

Commit and push. The post will appear on `/notes/` and homepage.
