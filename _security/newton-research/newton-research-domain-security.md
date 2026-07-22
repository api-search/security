---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: newtonresearch.ai
  spf: true
hosts:
- cert_expires: Sep 28 21:02:47 2026 GMT
  host: www.newtonresearch.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newton Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newton Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Newton Research
provider_slug: newton-research
slug: newton-research-domain-security
source_filename: newton-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newtonresearch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 21:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newtonresearch.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newton-research/refs/heads/main/security/newton-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Marketing Analytics
- MarTech
- AdTech
- AI Agents
- Data Science
- Analytics
---
