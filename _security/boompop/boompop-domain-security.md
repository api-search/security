---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: boompop.com
  spf: true
hosts:
- cert_expires: Oct  1 02:47:08 2026 GMT
  host: boompop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boompop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boompop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Boompop
provider_slug: boompop
slug: boompop-domain-security
source_filename: boompop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boompop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:47:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boompop.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boompop/refs/heads/main/security/boompop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Event Management
- Event Planning
- Corporate Events
- Hospitality
- Travel
- SaaS
- Meetings and Events
---
