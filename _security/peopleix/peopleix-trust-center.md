---
certifications:
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Peopleix Trust Center
name_suffix: Trust Center
overview: Peopleix maintains a public trust center documenting ISO 27001 and GDPR compliance.
provider_name: Peopleix
provider_slug: peopleix
slug: peopleix-trust-center
source_filename: peopleix-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://trust.peopleix.com (HTTP 200) and https://www.peopleix.com/llms.txt\nnote: >-\n  UPGRADE over the 2026-07-20 round, which recorded \"no dedicated trust portal found\".\n  peopleIX now operates a real trust center at https://trust.peopleix.com — HTTP 200,\n  canonical link rel points at itself, title \"peopleIX Trust Center\", hosted on Vanta\n  (content-location assets.vanta.com, EU tenant app.eu.vanta.com, trust-report slug\n  p1g8lgaeyivu1lc650i555). The certification and control inventory below is taken from\n  the page's own served metadata and from the llms.txt published on the same date. The\n  page body itself renders client-side (Vanta React SPA), so the individual document\n  list, sub-processor register and monitored-control counts could not be read without a\n  browser and are NOT recorded here — they are gated behind JS rendering, not behind a\n  login. The llms.txt describes the trust center as carrying \"\
  certificates, policies,\n  sub-processors\".\ntrust_center:\n  url: https://trust.peopleix.com\n  status: 200\n  platform: Vanta\n  platform_evidence: >-\n    content-location https://assets.vanta.com/static/vite/index-trust-report.vite...html;\n    og:image https://app.eu.vanta.com/doc?s=kk7ulk04wpdmr19cc1lfd; data-slugid\n    p1g8lgaeyivu1lc650i555.\n  region: EU tenant (app.eu.vanta.com)\n  rendering: client-side (JS-rendered SPA) — document inventory not machine-readable\ncertifications:\n- name: ISO 27001\n  status: certified\n  evidence: >-\n    \"ISO 27001 certified\" — llms.txt (2026-08-14 revision; the 2026-07-20 capture said\n    \"ISO 27001 compliant\", so this is a strengthened claim) and the trust center page\n    description.\n  auditor: not published\n  report_available: unknown\n- name: GDPR\n  status: claimed-compliant\n  evidence: \"'GDPR compliant'; EU-resident end-to-end (application, AI models, engineering).\"\ncontrols:\n- EU-resident application, AI models, and engineering\n\
  - AES-256 encryption at rest\n- TLS 1.2+ encryption in transit\n- Never trained on customer data\n- Permissioned by default — the customer decides who sees what\n- Conversations aggregate anonymously; employees never see each other's transcripts\ndocuments_published:\n  certificates: claimed (llms.txt names the trust center as carrying certificates)\n  policies: claimed\n  sub_processors: claimed\n  note: Named by peopleIX as trust-center contents; not independently readable because the page is JS-rendered.\nx-evidence:\n  fetched: '2026-08-14'\n  urls:\n  - url: https://trust.peopleix.com\n    status: 200\n    content_type: text/html\n  - url: https://www.peopleix.com/llms.txt\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleix/refs/heads/main/security/peopleix-trust-center.yml
summary_line: ISO 27001, GDPR
tags:
- Company
- HR
- People Analytics
- People Intelligence
- Conversation Intelligence
- Human Resources
- Workforce Analytics
- Artificial Intelligence
- MCP
- Germany
trust_url: ''
---
