---
api_specs:
- filename: finzdata-com-finzdata-api-openapi.yml
  format: yaml
  label: FinzData API
  slug: finzdata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finzdata-com/openapi/finzdata-com-finzdata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finzdata.com
  spf: true
hosts:
- cert_expires: Jan  8 16:00:00 2027 GMT
  host: finzdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 15:01:25 2027 GMT
  host: api.finzdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: FinzData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinzData, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FinzData
provider_slug: finzdata-com
slug: finzdata-com-domain-security
source_filename: finzdata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finzdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 16:00:00 2027 GMT\n  hsts: false\n- host: api.finzdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 15:01:25 2027 GMT\n  hsts: null\ndomains:\n- domain: finzdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/finzdata-com/security/finzdata-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Market Data
- Historical Data
- Python
---
