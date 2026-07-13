---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockfrost.io
  spf: true
hosts:
- cert_expires: Sep 18 14:17:05 2026 GMT
  host: blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockfrost Cardano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for blockfrost Cardano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: blockfrost Cardano
provider_slug: blockfrost-cardano
slug: blockfrost-cardano-domain-security
source_filename: blockfrost-cardano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockfrost.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockfrost-cardano/refs/heads/main/security/blockfrost-cardano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
