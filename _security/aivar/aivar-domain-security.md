---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aivar.tech
  spf: true
hosts:
- cert_expires: Sep  6 19:44:05 2026 GMT
  host: aivar.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aivar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aivar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aivar
provider_slug: aivar
slug: aivar-domain-security
source_filename: aivar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aivar.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:44:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aivar.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aivar/refs/heads/main/security/aivar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- AI Agents
- Consulting
- Voice AI
- Process Automation
- Kubernetes
---
