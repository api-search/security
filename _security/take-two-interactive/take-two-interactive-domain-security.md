---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: take2games.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.take2games.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.take2games.com
  https: false
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: api.take2games.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Take Two Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Take-Two Interactive Software, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Take-Two Interactive Software
provider_slug: take-two-interactive
slug: take-two-interactive-domain-security
source_filename: take-two-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.take2games.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.take2games.com\n  https: false\n- host: api.take2games.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: take2games.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/take-two-interactive/refs/heads/main/security/take-two-interactive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Entertainment
- Software
- Fortune 1000
---
