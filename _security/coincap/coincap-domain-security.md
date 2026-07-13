---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coincap.io
  spf: true
hosts:
- cert_expires: Sep  2 11:17:28 2026 GMT
  host: docs.coincap.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coincap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinCap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CoinCap
provider_slug: coincap
slug: coincap-domain-security
source_filename: coincap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.coincap.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 11:17:28 2026 GMT\n  hsts: false\ndomains:\n- domain: coincap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coincap/refs/heads/main/security/coincap-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Cryptocurrency
- Public APIs
---
