---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chevron.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.chevron.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chevron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chevron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chevron
provider_slug: chevron
slug: chevron-domain-security
source_filename: chevron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chevron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: chevron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chevron/refs/heads/main/security/chevron-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Caltex
- Chemicals
- Crude Oil
- Downstream
- Energy
- Fortune 500
- Houston
- Integrated Energy
- LNG
- Lubricants
- Natural Gas
- Petroleum
- Refining
- Renewable Fuels
- Texaco
- Upstream
---
