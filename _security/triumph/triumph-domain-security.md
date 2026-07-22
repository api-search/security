---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: triumphlabs.com
  spf: false
hosts:
- cert_expires: Oct 18 15:52:52 2026 GMT
  host: www.triumphlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Triumph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triumph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Triumph
provider_slug: triumph
slug: triumph-domain-security
source_filename: triumph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triumphlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:52:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: triumphlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triumph/refs/heads/main/security/triumph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Real-Money Gaming
- Tournaments
- Mobile Games
- SDK
- Payments
- Collectibles
---
