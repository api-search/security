---
certifications: []
description: ''
kind: trust-center
layout: security
name: Atera Trust Center
name_suffix: Trust Center
overview: Atera maintains a public trust center covering its security and compliance posture.
provider_name: Atera
provider_slug: atera
slug: atera-trust-center
source_filename: atera-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nprobe: true\nurl: https://trust.atera.com/\nplatform: Vanta Trust Center (EU tenant — app.eu.vanta.com)\nverified: true\nmachine_readable: false\nnotes: >-\n  trust.atera.com resolves and returns HTTP 200 with <title>Atera Trust Center</title>\n  and a canonical link to itself, served as a Vanta-hosted single-page app. The page\n  content — the certification list, subprocessors and document requests — is rendered\n  client-side from a GraphQL endpoint that rejects unsigned requests\n  (\"Missing `signature` or `signedAt`\", HTTP 400), so the certification roster could\n  NOT be read anonymously. Only certifications with an independent first-party source\n  are recorded as verified below; the rest are deliberately left unasserted rather than\n  copied from secondhand summaries.\n\ncertifications_verified:\n- name: SOC 2 Type 2\n  source: https://community.atera.com/discussion/335/were-officially-soc-2-type-2-certified\n  source_type:\
  \ Atera admin announcement on Atera's own community\n  announced: '2024-01'\n\ncertifications_unverified:\n  note: >-\n    Third-party summaries of trust.atera.com list ISO/IEC 27001, 27017, 27018, 27032 and\n    42001, HIPAA, GDPR and CCPA alongside SOC 2 Type 2. These could not be confirmed\n    against a page this pipeline could actually read, so they are recorded as unverified\n    rather than claimed.\n\nsubprocessors:\n  url: https://trust.atera.com/subprocessors\n  status: 200\n  readable: false\n  note: SPA route; returns the same client-rendered shell.\n\nevidence:\n- {source: 'https://trust.atera.com/', http_status: 200, title: 'Atera Trust Center', vendor: vanta, fetched: '2026-08-06'}\n- {source: 'https://trust.atera.com/graphql', http_status: 400, error: 'Missing `signature` or `signedAt`', fetched: '2026-08-06'}\n- {source: 'https://community.atera.com/discussion/335/were-officially-soc-2-type-2-certified', http_status: 200, fetched: '2026-08-06'}\n\ngaps:\n- >-\n  The trust\
  \ center is not machine-readable: no JSON, no feed, and a request-signed\n  GraphQL API. An agent evaluating Atera's compliance posture cannot read it.\n- No /.well-known/security.txt on any Atera host (see well-known/atera-well-known.yml).\n- No published vulnerability disclosure policy or bug bounty program was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atera/refs/heads/main/security/atera-trust-center.yml
summary_line: trust center published
tags:
- IT Management
- RMM
- PSA
- Help Desk
- Ticketing
- Patch Management
- Remote Monitoring
- Endpoint Management
- MSP
- Network Discovery
- Alerts
- Devices
- Billing
- Webhook
- Artificial Intelligence
trust_url: https://trust.atera.com/
---
