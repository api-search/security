---
api_specs:
- filename: trabex-trade-compliance-openapi.yml
  format: yaml
  label: Trabex Trade Compliance API
  slug: trade-compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/openapi/trabex-trade-compliance-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trabex.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: trabex.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 09:52:53 2026 GMT
  host: apidocs.trabex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.trabex.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trabex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trabex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trabex
provider_slug: trabex
slug: trabex-domain-security
source_filename: trabex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trabex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: apidocs.trabex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:52:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trabex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trabex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trabex/refs/heads/main/security/trabex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Export Control
- Logistics
- Restricted Party Screening
- Shipment Management
- Trade Compliance
---
