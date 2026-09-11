---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foodvisor.io
  note: 'SPF corrected by hand 2026-09-10 after verification with `dig TXT foodvisor.io`. probe-domain-security.py recorded spf: false on two consecutive runs; its dig call uses +time=2 +tries=1, which intermittently times out against this domain''s eight-record TXT set and silently yields a false negative. The record is present.'
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:mail.zendesk.com ~all
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.foodvisor.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foodvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foodvisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foodvisor
provider_slug: foodvisor
slug: foodvisor-domain-security
source_filename: foodvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foodvisor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foodvisor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:mail.zendesk.com\n    ~all\n  note: 'SPF corrected by hand 2026-09-10 after verification with `dig TXT foodvisor.io`. probe-domain-security.py\n    recorded spf: false on two consecutive runs; its dig call uses +time=2 +tries=1, which intermittently\n    times out against this domain''s eight-record TXT set and silently yields a false negative. The record\n    is present.'\nnote: 'method: probed, with one hand-verified correction — see domains[].note for foodvisor.io. No value\n  here was assumed; each was read from a live\
  \ DNS or TLS response.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foodvisor/refs/heads/main/security/foodvisor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Computer-Vision
- Food
- Health
- Nutrition
- Mobile
---
