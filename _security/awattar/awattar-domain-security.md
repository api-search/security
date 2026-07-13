---
api_specs:
- filename: openapi.yml
  format: yaml
  label: aWATTar Market Data API
  slug: awattar-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awattar/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: awattar.at
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: awattar.de
  spf: true
hosts:
- cert_expires: Aug  7 20:32:18 2026 GMT
  host: www.awattar.at
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  7 20:32:18 2026 GMT
  host: api.awattar.at
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  7 20:33:34 2026 GMT
  host: api.awattar.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Awattar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aWATTar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aWATTar
provider_slug: awattar
slug: awattar-domain-security
source_filename: awattar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.awattar.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 20:32:18 2026 GMT\n  hsts: false\n- host: api.awattar.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 20:32:18 2026 GMT\n  hsts: null\n- host: api.awattar.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 20:33:34 2026 GMT\n  hsts: null\ndomains:\n- domain: awattar.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: awattar.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awattar/refs/heads/main/security/awattar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electricity
- Energy
- Spot Price
- EPEX Spot
- Dynamic Pricing
- Austria
- Germany
- Smart Energy
- IoT
---
