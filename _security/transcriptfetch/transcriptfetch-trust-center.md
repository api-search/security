---
api_specs:
- filename: transcriptfetch-api-v2-openapi.json
  format: json
  label: TranscriptFetch REST API
  slug: transcriptfetch-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/openapi/transcriptfetch-api-v2-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Transcriptfetch Trust Center
name_suffix: Trust Center
overview: TranscriptFetch maintains a public trust center covering its security and compliance posture.
provider_name: TranscriptFetch
provider_slug: transcriptfetch
slug: transcriptfetch-trust-center
source_filename: transcriptfetch-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nprobe: true\nsource: https://transcriptfetch.com/trust\nurl: https://transcriptfetch.com/trust\nnote: >-\n  The trust page explicitly states TranscriptFetch is NOT SOC 2 or ISO 27001 certified\n  and holds no BAA or FedRAMP authorization — the keyword probe's SOC 2 / ISO 27001\n  matches were the disclaimer sentence, not claims. What IS published: a CSA STAR\n  Registry Level 1 CAIQ v4 self-assessment answering all 261 Cloud Controls Matrix\n  questions, an independent third-party status page, public shallow + deep health\n  endpoints, a full subprocessor list, and a 12-month versioning/deprecation commitment.\ncertifications: []\nself_assessments:\n- name: CSA STAR Level 1 (CAIQ v4 self-assessment)\n  registry: https://cloudsecurityalliance.org/star/registry/transcriptfetch\n  detail: Answers all 261 Cloud Controls Matrix questions; published on the Cloud Security Alliance STAR Registry (verified HTTP 200 2026-09-09).\ndisclaimed:\n\
  - SOC 2\n- ISO 27001\n- BAA (HIPAA)\n- FedRAMP\nprivacy:\n  gdpr_ccpa: Honours GDPR and CCPA data rights requests (stated on /security).\n  data_use: No sale of personal data; transcript requests are not used to train models.\nsubprocessors:\n- {name: Clerk, purpose: Authentication}\n- {name: Neon, purpose: Postgres database}\n- {name: Stripe, purpose: Payments}\n- {name: Cloudflare, purpose: DNS, note: CDN + TLS termination + outbound tunnel (no exposed origin)}\n- {name: DeepInfra, purpose: Speech recognition for videos with no captions}\n- {name: Resend, purpose: Transactional email}\n- {name: Better Stack, purpose: Uptime monitoring}\n- {name: Microsoft Clarity, purpose: Product analytics}\nevidence:\n- source: https://transcriptfetch.com/trust\n  detail: \"'We are not SOC 2 or ISO 27001 certified. If your procurement needs that, say so...'\"\n- source: https://transcriptfetch.com/security\n  detail: \"'TranscriptFetch is not currently SOC 2 or ISO 27001 certified, and we do not have\
  \ a signed BAA or FedRAMP authorisation.'\"\n- source: https://cloudsecurityalliance.org/star/registry/transcriptfetch\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/security/transcriptfetch-trust-center.yml
summary_line: trust center published
tags:
- transcripts
- speech-to-text
- captions
- youtube
- tiktok
- instagram
- podcasts
- mcp
- llms-txt
- openapi
- Transcription
- Speech-to-Text
- Video
- Podcasts
- AI/LLM
- RAG
- Agents
- MCP
- Developer Tools
- Media
- Content
- YouTube
- TikTok
- Instagram
- Spotify
- Apple Podcasts
trust_url: https://transcriptfetch.com/trust
---
