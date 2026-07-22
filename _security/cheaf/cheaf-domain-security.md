---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cheaf.com
  spf: true
hosts:
- cert_expires: Aug 29 20:17:19 2026 GMT
  host: cheaf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cheaf
provider_slug: cheaf
slug: cheaf-domain-security
source_filename: cheaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheaf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cheaf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheaf/refs/heads/main/security/cheaf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food Tech
- Marketplace
- Food Waste
- Sustainability
- Retail
- Mobile App
- Latin America
---
