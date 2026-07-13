---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wework.com
  spf: true
hosts:
- cert_expires: Sep  7 15:11:10 2026 GMT
  host: www.wework.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 14:47:16 2026 GMT
  host: developers.wework.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeWork, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WeWork
provider_slug: wework
slug: wework-domain-security
source_filename: wework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:11:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.wework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:47:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wework.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wework/refs/heads/main/security/wework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coworking
- Flexible Workspace
- Real Estate
- Workspace Booking
- Workplace Management
- Bookings
- Inventory
---
