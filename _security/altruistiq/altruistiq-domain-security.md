---
api_specs:
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq Datasource API
  slug: altruistiq-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq PACT API
  slug: altruistiq-pact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altruistiq.com
  spf: true
hosts:
- cert_expires: Oct  1 03:57:05 2026 GMT
  host: www.altruistiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 20:04:53 2026 GMT
  host: docs.altruistiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 20:04:53 2026 GMT
  host: app.altruistiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altruistiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altruistiq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Altruistiq
provider_slug: altruistiq
slug: altruistiq-domain-security
source_filename: altruistiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altruistiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:57:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.altruistiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:04:53 2026 GMT\n  hsts: false\n- host: app.altruistiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:04:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: altruistiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/security/altruistiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sustainability
- Climate
- Carbon Accounting
- Emissions
- Greenhouse Gas
- Scope 3
- Product Carbon Footprint
- Corporate Carbon Footprint
- Supply Chain
- FMCG
- Food and Beverage
- ESG
- CSRD
- SBTi
- PACT
- Sustainability Intelligence
---
