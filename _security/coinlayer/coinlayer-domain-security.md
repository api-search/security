---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coinlayer.com
  spf: true
hosts:
- cert_expires: Sep  2 18:41:19 2026 GMT
  host: coinlayer.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinlayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coinlayer
provider_slug: coinlayer
slug: coinlayer-domain-security
source_filename: coinlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:41:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: coinlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlayer/refs/heads/main/security/coinlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
