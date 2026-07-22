---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: movius.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moviuscorp.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: movius.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:43:06 2026 GMT
  host: help.moviuscorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Movius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Movius, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Movius
provider_slug: movius
slug: movius-domain-security
source_filename: movius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movius.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.moviuscorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: movius.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moviuscorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movius/refs/heads/main/security/movius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Messaging
- Mobile
- Telecom
- Compliance
- Security
- Voice
- SMS
- Enterprise
---
