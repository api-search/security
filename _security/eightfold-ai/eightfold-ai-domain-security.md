---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eightfold.ai
  spf: true
hosts:
- cert_expires: Sep 17 19:59:24 2026 GMT
  host: eightfold.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: app.eightfold.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eightfold Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eightfold AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eightfold AI
provider_slug: eightfold-ai
slug: eightfold-ai-domain-security
source_filename: eightfold-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eightfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:59:24 2026 GMT\n  hsts: false\n- host: app.eightfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eightfold.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eightfold-ai/refs/heads/main/security/eightfold-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Talent Intelligence
- Talent Acquisition
- Talent Management
- AI Interviewing
- HR Tech
- Workforce Planning
- Agentic AI
---
