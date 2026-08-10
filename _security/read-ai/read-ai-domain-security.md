---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: read.ai
  spf: true
hosts:
- cert_expires: Oct 14 20:50:41 2026 GMT
  host: www.read.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:44:55 2026 GMT
  host: support.read.ai
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.read.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Read Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Read AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Read AI
provider_slug: read-ai
slug: read-ai-domain-security
source_filename: read-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.read.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:50:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.read.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:44:55 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.read.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: read.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/read-ai/refs/heads/main/security/read-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Meeting Intelligence
- Artificial Intelligence
- Transcription
- Productivity
- Collaboration
- Model Context Protocol
- Agents
- Webhooks
- SaaS
---
