---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brandback.ai
  spf: true
hosts:
- cert_expires: Oct  8 22:18:28 2026 GMT
  host: www.brandback.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandback, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brandback
provider_slug: brandback
slug: brandback-domain-security
source_filename: brandback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandback.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brandback.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandback/refs/heads/main/security/brandback-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Resale
- Recommerce
- E-commerce
- Retail
- Sustainability
- Fashion
- Circular Economy
---
