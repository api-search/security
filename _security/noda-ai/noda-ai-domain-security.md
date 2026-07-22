---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: nodaintelligence.ai
  spf: true
hosts:
- cert_expires: Oct  5 04:50:12 2026 GMT
  host: www.nodaintelligence.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noda Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NODA AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NODA AI
provider_slug: noda-ai
slug: noda-ai-domain-security
source_filename: noda-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nodaintelligence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:50:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nodaintelligence.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noda-ai/refs/heads/main/security/noda-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Deep Tech
- Defense
- Defense Technology
- Autonomy
- Artificial Intelligence
- Orchestration
- Military
- Robotics
---
