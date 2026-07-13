---
api_specs:
- filename: swagger.json
  format: json
  label: Elexon Insights Solution API
  slug: insights-solution-api
  spec_type: OpenAPI
  url: https://data.elexon.co.uk/swagger/v1/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elexon.co.uk
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: developer.data.elexon.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: data.elexon.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elexon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elexon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elexon
provider_slug: elexon
slug: elexon-domain-security
source_filename: elexon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.data.elexon.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.elexon.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: elexon.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elexon/refs/heads/main/security/elexon-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Electricity
- Energy
- UK Energy Market
- Balancing Mechanism
- Settlement
- Meter Readings
- Market Transparency
- BMRS
- Electricity Grid
- Power Generation
- United Kingdom
---
