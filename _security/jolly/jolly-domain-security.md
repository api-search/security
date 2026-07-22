---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jolly.com
  spf: true
hosts:
- cert_expires: Aug 19 21:48:09 2026 GMT
  host: jolly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jolly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jolly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jolly
provider_slug: jolly
slug: jolly-domain-security
source_filename: jolly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jolly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:48:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jolly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jolly/refs/heads/main/security/jolly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workforce Engagement
- Employee Rewards
- Gamification
- HR Tech
- Frontline Workforce
- Workforce Management
- Recruiting
- Incentives
---
