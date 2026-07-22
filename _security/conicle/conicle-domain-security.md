---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conicle.com
  spf: true
hosts:
- cert_expires: Sep  8 12:52:37 2026 GMT
  host: conicle.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conicle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conicle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conicle
provider_slug: conicle
slug: conicle-domain-security
source_filename: conicle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conicle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:52:37 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: conicle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conicle/refs/heads/main/security/conicle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EdTech
- Learning Management System
- Corporate Training
- E-Learning
- Design System
- Thailand
---
