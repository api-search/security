---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mirado.ai
  spf: false
hosts:
- cert_expires: Sep  8 11:51:20 2026 GMT
  host: mirado.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mirado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mirado
provider_slug: mirado
slug: mirado-domain-security
source_filename: mirado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mirado.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mirado.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirado/refs/heads/main/security/mirado-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Rewards
- Loyalty
- Card-Linked Offers
- Advertising
- MarTech
- Publishers
- Fintech
---
