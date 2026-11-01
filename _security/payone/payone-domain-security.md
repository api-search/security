---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payone.com
  spf: true
hosts:
- cert_expires: Jan 21 17:52:04 2027 GMT
  host: payone.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Payone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PAYONE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PAYONE
provider_slug: payone
slug: payone-domain-security
source_filename: payone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 17:52:04 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: payone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/payone/security/payone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- E‑Commerce
- Point‑of‑Sale
- Card Payments
- Retail
- Hospitality
---
