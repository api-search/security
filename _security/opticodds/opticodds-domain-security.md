---
api_specs:
- filename: opticodds-openapi.yml
  format: yaml
  label: OpticOdds
  slug: opticodds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opticodds/refs/heads/main/openapi/opticodds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opticodds.com
  spf: false
hosts:
- cert_expires: Oct  6 22:18:51 2026 GMT
  host: opticodds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 10:52:20 2026 GMT
  host: api.opticodds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opticodds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpticOdds, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OpticOdds
provider_slug: opticodds
slug: opticodds-domain-security
source_filename: opticodds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opticodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:18:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opticodds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:52:20 2026 GMT\n  hsts: null\ndomains:\n- domain: opticodds.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opticodds/refs/heads/main/security/opticodds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Odds
- Sports Betting
- Sports Data
---
