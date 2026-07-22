---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workhuman.com
  spf: true
hosts:
- cert_expires: Oct  4 14:46:27 2026 GMT
  host: www.workhuman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workhuman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workhuman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workhuman
provider_slug: workhuman
slug: workhuman-domain-security
source_filename: workhuman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workhuman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:46:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workhuman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workhuman/refs/heads/main/security/workhuman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Recognition
- Human Resources
- Employee Engagement
- Rewards
- People Analytics
- SaaS
---
