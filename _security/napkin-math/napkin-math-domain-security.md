---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: napkinmath.club
  spf: true
hosts:
- cert_expires: Aug 23 13:34:54 2026 GMT
  host: napkinmath.club
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Napkin Math Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Napkin Math, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Napkin Math
provider_slug: napkin-math
slug: napkin-math-domain-security
source_filename: napkin-math-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: napkinmath.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:34:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: napkinmath.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkin-math/refs/heads/main/security/napkin-math-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Food Journal
- Health
- Diet
- Artificial Intelligence
- Consumer Application
- Mobile Application
- iOS
---
