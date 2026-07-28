---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hydroone.com
  spf: true
hosts:
- cert_expires: Jan 29 15:18:51 2027 GMT
  host: www.hydroone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydro One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydro One, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hydro One
provider_slug: hydro-one
slug: hydro-one-domain-security
source_filename: hydro-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hydroone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 15:18:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hydroone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-one/refs/heads/main/security/hydro-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Smart Metering
- Green Button
- Energy Data
- Transmission
- Distribution
---
