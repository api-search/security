---
api_specs:
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital ClearAVM / Valuation API
  slug: clearavm-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Comparables (Comps) API
  slug: comps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
- filename: clear-capital-openapi.yml
  format: yaml
  label: Clear Capital Appraisal & Orders API
  slug: appraisal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/openapi/clear-capital-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearcapital.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.clearcapital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.clearcapital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clear Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Capital, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clear Capital
provider_slug: clear-capital
slug: clear-capital-domain-security
source_filename: clear-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clearcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearcapital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-capital/refs/heads/main/security/clear-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Data
- Valuation
- AVM
- Appraisal
- Mortgage
---
