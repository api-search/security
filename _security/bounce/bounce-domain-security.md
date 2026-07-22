---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bounce.com
  spf: true
hosts:
- cert_expires: Sep 27 21:43:58 2026 GMT
  host: bounce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bounce
provider_slug: bounce
slug: bounce-domain-security
source_filename: bounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bounce.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounce/refs/heads/main/security/bounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Luggage Storage
- Travel
- Marketplace
- Logistics
- Consumer
- Storage Network
- Hospitality
---
