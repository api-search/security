---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zerolongevity.com
  spf: true
hosts:
- cert_expires: Sep  8 22:20:53 2026 GMT
  host: zerolongevity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Big Sky Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Sky Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Big Sky Health
provider_slug: big-sky-health
slug: big-sky-health-domain-security
source_filename: big-sky-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zerolongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:20:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zerolongevity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-sky-health/refs/heads/main/security/big-sky-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Fasting
- Nutrition
- Longevity
- Consumer App
- Mobile
---
