---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mai.co
  spf: true
hosts:
- cert_expires: Oct  6 08:40:15 2026 GMT
  host: www.mai.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MAI
provider_slug: mai
slug: mai-domain-security
source_filename: mai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:40:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mai.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mai/refs/heads/main/security/mai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Artificial Intelligence
- Marketing
- Advertising
- Performance Marketing
- AI Agents
- Digital Advertising
- MarTech
- Google Ads
---
