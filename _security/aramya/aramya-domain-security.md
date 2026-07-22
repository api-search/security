---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aramya.in
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: aramya.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aramya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aramya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Aramya
provider_slug: aramya
slug: aramya-domain-security
source_filename: aramya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aramya.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aramya.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramya/refs/heads/main/security/aramya-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Fashion
- Ecommerce
- Retail
- D2C
- Apparel
- India
---
