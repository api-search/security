---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daash.co
  spf: false
hosts:
- cert_expires: Oct  1 06:57:38 2026 GMT
  host: daash.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Daash
provider_slug: daash
slug: daash-domain-security
source_filename: daash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daash.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:57:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: daash.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daash/refs/heads/main/security/daash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Competitive Intelligence
- Market Intelligence
- Beauty
- Cosmetics
- Consumer Products
- Retail Analytics
- Predictive Analytics
- SaaS
---
