---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: noteworthy.ai
  spf: true
hosts:
- cert_expires: Sep 11 04:46:52 2026 GMT
  host: noteworthy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noteworthy Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noteworthy AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Noteworthy AI
provider_slug: noteworthy-ai
slug: noteworthy-ai-domain-security
source_filename: noteworthy-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noteworthy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noteworthy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noteworthy-ai/refs/heads/main/security/noteworthy-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Machine Learning
- Electric Utilities
- Grid Inspection
- Energy
- Infrastructure
---
