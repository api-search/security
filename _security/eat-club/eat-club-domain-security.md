---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eatclub.com
  spf: true
hosts:
- cert_expires: Sep 25 00:43:14 2026 GMT
  host: www.eatclub.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eat Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EAT Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EAT Club
provider_slug: eat-club
slug: eat-club-domain-security
source_filename: eat-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eatclub.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 00:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: eatclub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eat-club/refs/heads/main/security/eat-club-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Food Service
- Corporate Catering
- Meal Delivery
- Food Tech
- Workplace
- Employee Benefits
- Logistics
- Hospitality
---
