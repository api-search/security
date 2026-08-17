---
certifications: []
description: ''
kind: trust-center
layout: security
name: Sprinter Health Trust Center
name_suffix: Trust Center
overview: Sprinter Health maintains a public trust center covering its security and compliance posture.
provider_name: Sprinter Health
provider_slug: sprinter-health
slug: sprinter-health-trust-center
source_filename: sprinter-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nprobe: true\nurl: https://trust.sprinterhealth.com/\nplatform: Vanta Trust Center\ncertifications: []\nnote: >-\n  A trust center is served at trust.sprinterhealth.com — HTTP 200, a Vanta-hosted\n  page whose served HTML carries <title>Sprinter Health Trust Center</title> and the\n  Vanta asset/manifest references. Its CONTENT (control framework list, certifications,\n  documents) is rendered client-side and its backing GraphQL API is request-signed:\n  POST https://trust.sprinterhealth.com/graphql returns HTTP 400\n  {\"errors\":[{\"message\":\"Missing `signature` or `signedAt`\"}]}. No certification could\n  therefore be read from the served bytes, so certifications[] is an honest empty list\n  rather than a guess. NO `Compliance` pointer is emitted: the existence of a trust\n  center is verified, a published certification is not.\nevidence:\n  - source: https://trust.sprinterhealth.com/\n    http_status: 200\n    kind: trust-center-page\n\
  \    keywords: [trust, security, compliance]\n    detail: 'Vanta-hosted; <title>Sprinter Health Trust Center</title>'\n  - source: https://trust.sprinterhealth.com/graphql\n    http_status: 400\n    kind: trust-center-api\n    detail: 'signature-gated: {\"message\":\"Missing `signature` or `signedAt`\"}'\nx-evidence:\n  fetched: '2026-08-15'\n  url: https://trust.sprinterhealth.com/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprinter-health/refs/heads/main/security/sprinter-health-trust-center.yml
summary_line: trust center published
tags:
- Company
- Health
- Healthcare
- In-Home Care
- Preventive Care
- Diagnostics
- Telehealth
- Care Navigation
trust_url: https://trust.sprinterhealth.com/
---
