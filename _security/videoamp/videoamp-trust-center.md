---
api_specs:
- filename: videoamp-public-api-openapi.yml
  format: yaml
  label: VideoAmp Public API
  slug: videoamp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-public-api-openapi.yml
certifications: []
description: VideoAmp operates a Vanta-hosted trust center at trust.videoamp.com. The host resolves and returns HTTP 200, and the served document is a Vanta trust report shell (data-signature-manifest-url on assets.vanta.com, meta keywords "Trust, Security, Compliance, Automation", slug id kc0vaj770r912yhumz0k2). The page body is rendered entirely client-side, so the certification list, subprocessor list and document library could not be read anonymously.
kind: trust-center
layout: security
name: Videoamp Trust Center
name_suffix: Trust Center
overview: VideoAmp maintains a public trust center covering its security and compliance posture.
provider_name: VideoAmp
provider_slug: videoamp
slug: videoamp-trust-center
source_filename: videoamp-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nprobe: true\nurl: https://trust.videoamp.com/\nplatform: Vanta\ndescription: >-\n  VideoAmp operates a Vanta-hosted trust center at trust.videoamp.com. The host resolves and returns\n  HTTP 200, and the served document is a Vanta trust report shell (data-signature-manifest-url on\n  assets.vanta.com, meta keywords \"Trust, Security, Compliance, Automation\", slug id\n  kc0vaj770r912yhumz0k2). The page body is rendered entirely client-side, so the certification list,\n  subprocessor list and document library could not be read anonymously.\ncertifications: []\ncertifications_note: >-\n  NOT verified. The 3.5 KB HTML shell served to an anonymous fetch contains no certification names.\n  Reading the actual compliance posture requires a JavaScript-rendering client or a Vanta access\n  request. Do not assert SOC 2 / ISO 27001 / HIPAA / PCI for VideoAmp on the basis of this artifact.\ndocuments_gated: true\nevidence:\n  - source: https://trust.videoamp.com/\n\
  \    http_status: 200\n    content_type: text/html\n    keywords: [trust, security, compliance]\n    platform_markers:\n      - assets.vanta.com/static/index-trust-report.css\n      - data-signature-manifest-url=https://assets.vanta.com/static/signature-manifest...\n      - data-slugid=kc0vaj770r912yhumz0k2\n  - source: https://trust.videoamp.com/.well-known/security.txt\n    http_status: 200\n    content_type: text/html\n    valid: false\n    note: SPA catch-all returns the same HTML shell for every path — not a real security.txt.\nrelated:\n  vulnerability_disclosure: security/videoamp-vulnerability-disclosure.yml\nx-evidence:\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/security/videoamp-trust-center.yml
summary_line: trust center published
tags:
- media-measurement
- advertising
- adtech
- tv-currency
- audience-measurement
- media-planning
- streaming
- attribution
- data-collaboration
- mcp
- agent-native
trust_url: https://trust.videoamp.com/
---
