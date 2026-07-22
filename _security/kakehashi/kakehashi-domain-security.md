---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kakehashi.life
  spf: true
hosts:
- cert_expires: Sep 24 23:34:08 2026 GMT
  host: kakehashi.life
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kakehashi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kakehashi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kakehashi
provider_slug: kakehashi
slug: kakehashi-domain-security
source_filename: kakehashi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kakehashi.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:34:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kakehashi.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakehashi/refs/heads/main/security/kakehashi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- SaaS
- Japan
- Medication
- Digital Health
- Inventory Management
---
