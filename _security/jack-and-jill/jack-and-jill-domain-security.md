---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jackandjill.ai
  spf: true
hosts:
- cert_expires: Oct  2 04:10:30 2026 GMT
  host: jackandjill.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jack And Jill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jack & Jill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jack & Jill
provider_slug: jack-and-jill
slug: jack-and-jill-domain-security
source_filename: jack-and-jill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jackandjill.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:10:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jackandjill.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jack-and-jill/refs/heads/main/security/jack-and-jill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Recruiting
- Hiring
- Talent
- HR Tech
- AI Agents
- Job Search
- Recruitment
---
