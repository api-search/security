---
api_specs:
- filename: landcor-property-api-openapi.json
  format: json
  label: Landcor Property API
  slug: landcor-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-property-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: landcor.com
  spf: true
hosts:
- cert_expires: Sep 17 15:03:17 2026 GMT
  host: www.landcor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.landcor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landcor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landcor Data, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Landcor Data
provider_slug: landcor
slug: landcor-domain-security
source_filename: landcor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:03:17 2026 GMT\n  hsts: false\n- host: api.landcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: landcor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/security/landcor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- Canada
- Valuation
- AVM
- Property Records
- Title
- Land Registry
- Mortgage
- PropTech
- Property Data
---
