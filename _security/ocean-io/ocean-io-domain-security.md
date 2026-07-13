---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ocean.io
  spf: true
hosts:
- cert_expires: Aug 12 13:34:28 2026 GMT
  host: ocean.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 13:34:28 2026 GMT
  host: api.ocean.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocean Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ocean.io
provider_slug: ocean-io
slug: ocean-io-domain-security
source_filename: ocean-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocean.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ocean.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ocean.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/security/ocean-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Intelligence
- B2B
- Enrichment
- Lookalike
- ABM
- Prospecting
---
