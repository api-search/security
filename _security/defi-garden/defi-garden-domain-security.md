---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: defi.garden
  spf: true
hosts:
- cert_expires: Jan  3 03:50:17 2027 GMT
  host: defi.garden
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defi Garden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeFi Garden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: DeFi Garden
provider_slug: defi-garden
slug: defi-garden-domain-security
source_filename: defi-garden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defi.garden\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:50:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: defi.garden\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/defi-garden/security/defi-garden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- DeFi
- Crypto Data
- Token Yields
- Chain Yields
---
