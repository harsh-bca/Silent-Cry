---
title: Silent Cry API Documentation
language_tabs:
  - shell
  - python
  - javascript
toc_footers:
  - <a href='mailto:contact@silentcry.in'>Contact Support</a>
  - <a href='https://github.com/yourusername/silentcry'>View on GitHub</a>
includes:
  - errors
search: true
---

# Introduction

Silent Cry is a mobile-first application enabling anonymous child abuse reporting with built-in mental health support and AI-powered sentiment tagging.

This API lets verified NGOs, psychologists, or child safety authorities connect and access anonymized data (with permissions).

# Authentication

```shell
curl -X POST https://api.silentcry.in/auth \
  -H "Content-Type: application/json" \
  -d '{"api_key": "your_api_key"}'
