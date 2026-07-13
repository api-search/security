---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geocod.io
  spf: true
hosts:
- cert_expires: Oct  3 13:30:28 2026 GMT
  host: www.geocod.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocod Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocod.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geocod.io
provider_slug: geocod-io
slug: geocod-io-domain-security
source_filename: geocod-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geocod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geocod.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocod-io/refs/heads/main/security/geocod-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Public APIs
---
