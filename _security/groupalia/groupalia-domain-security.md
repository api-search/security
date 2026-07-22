---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groupalia.it
  spf: true
hosts:
- cert_expires: Sep  1 17:26:35 2026 GMT
  host: www.groupalia.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groupalia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groupalia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groupalia
provider_slug: groupalia
slug: groupalia-domain-security
source_filename: groupalia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groupalia.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: groupalia.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupalia/refs/heads/main/security/groupalia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Daily Deals
- Group Buying
- E-commerce
- Gift Cards
- Retail
- Spain
---
