---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: novig.us
  spf: false
hosts:
- cert_expires: Oct 14 22:51:09 2026 GMT
  host: novig.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Novig
provider_slug: novig
slug: novig-domain-security
source_filename: novig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novig.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: novig.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novig/refs/heads/main/security/novig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Sports Betting
- Prediction Markets
- Trading
- Consumer App
---
