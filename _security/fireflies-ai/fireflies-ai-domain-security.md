---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fireflies.ai
  spf: true
hosts:
- cert_expires: Sep 11 13:20:39 2026 GMT
  host: docs.fireflies.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:04:16 2026 GMT
  host: api.fireflies.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fireflies Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fireflies.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fireflies.ai
provider_slug: fireflies-ai
slug: fireflies-ai-domain-security
source_filename: fireflies-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.fireflies.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:20:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fireflies.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:04:16 2026 GMT\n  hsts: null\ndomains:\n- domain: fireflies.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireflies-ai/refs/heads/main/security/fireflies-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Meetings
- Transcription
- Speech to Text
- Conversation Intelligence
- Artificial Intelligence
- GraphQL
- MCP
- Productivity
---
