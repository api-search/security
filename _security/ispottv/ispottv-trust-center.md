---
certifications: []
description: ''
kind: trust-center
layout: security
name: Ispottv Trust Center
name_suffix: Trust Center
overview: iSpot.tv maintains a public trust center covering its security and compliance posture.
provider_name: iSpot.tv
provider_slug: ispottv
slug: ispottv-trust-center
source_filename: ispottv-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://www.ispot.tv/ (homepage footer link) + https://trust.ispot.tv/\nurl: https://trust.ispot.tv/\n# trust.ispot.tv is a live, dedicated trust-center subdomain linked from the iSpot.tv\n# homepage footer. The portal returns HTTP 403 to automated clients, so named\n# certifications (SOC 2 / ISO 27001 / etc.) could not be captured verbatim and are\n# intentionally left empty rather than fabricated.\ncertifications: []\nevidence:\n  - source: https://www.ispot.tv/\n    keywords: [trust center, security]\n  - source: https://trust.ispot.tv/\n    status: 403\n    note: dedicated trust-center subdomain resolves; body gated to automated clients\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispottv/refs/heads/main/security/ispottv-trust-center.yml
summary_line: trust center published
tags:
- Company
- TV Advertising
- Advertising Measurement
- Analytics
- Attribution
- Media
- Marketing
- Streaming
trust_url: https://trust.ispot.tv/
---
