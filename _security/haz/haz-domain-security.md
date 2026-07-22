---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haz.co
  spf: true
hosts:
- cert_expires: Sep  5 00:25:12 2026 GMT
  host: www.haz.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Haz
provider_slug: haz
slug: haz-domain-security
source_filename: haz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.haz.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:25:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: haz.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haz/refs/heads/main/security/haz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Commerce
- Resale
- Marketplace
- Consumer
- Mobile App
- Artificial Intelligence
- Secondhand
- E-Commerce
---
