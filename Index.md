---
title: Silent Cry API Documentation
language_tabs:
  - shell
  - python
  - javascript
toc_footers:
  - <a href='mailto:contact@silent-cry.in'>Contact Support</a>
  - <a href='https://github.com/harsh-bca/silent-cry'>View on GitHub</a>
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
POST /complaint

Payload:
{
  "type": "voice" | "text",
  "content": "...",
  "language": "en" | "hi",
  "timestamp": "...",
  "device_id": "anonymized"
}
# POST /api/v1/report
curl -X POST https://api.silentcry.in/api/v1/report \
  -H "Authorization: Bearer your_token" \
  -H "Content-Type: application/json" \
  -d '{
    "reporter_id": "12345",
    "incident_type": "physical_abuse",
    "incident_details": "Details about the incident",
    "location": "City, Country"
  }'





