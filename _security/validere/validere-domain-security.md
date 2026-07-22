---
api_specs:
- filename: validere-carbonhub-openapi-original.json
  format: json
  label: Validere CarbonHub App API
  slug: validere-carbonhub-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/openapi/validere-carbonhub-openapi-original.json
- filename: validere-dataplatform-source-openapi-original.json
  format: json
  label: Validere Data Platform Source API
  slug: validere-data-platform-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/openapi/validere-dataplatform-source-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: validere.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: validere.io
  spf: false
hosts:
- cert_expires: Aug  2 19:40:29 2026 GMT
  host: validere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:25:04 2026 GMT
  host: api.validere.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Validere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Validere, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Validere
provider_slug: validere
slug: validere-domain-security
source_filename: validere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 19:40:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.validere.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:25:04 2026 GMT\n  hsts: null\ndomains:\n- domain: validere.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: validere.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/security/validere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Applications
- Energy
- Emissions
- Methane
- Oil And Gas
- Environmental Data
- Measurement
- Carbon Intensity
- EHS
---
