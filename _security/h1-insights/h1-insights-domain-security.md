---
api_specs:
- filename: h1-insights-cost-estimates-api-openapi.yml
  format: yaml
  label: H1 Cost Estimates API
  slug: h1-insights-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-cost-estimates-api-openapi.yml
- filename: h1-insights-filters-api-openapi.yml
  format: yaml
  label: H1 Filters API
  slug: h1-insights-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-filters-api-openapi.yml
- filename: h1-insights-focus-area-endpoints-api-openapi.yml
  format: yaml
  label: H1 Focus Area Endpoints API
  slug: h1-insights-focus-area-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-focus-area-endpoints-api-openapi.yml
- filename: h1-insights-locations-api-openapi.yml
  format: yaml
  label: H1 Locations API
  slug: h1-insights-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-locations-api-openapi.yml
- filename: h1-insights-networks-api-openapi.yml
  format: yaml
  label: H1 Networks API
  slug: h1-insights-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-networks-api-openapi.yml
- filename: h1-insights-organizations-api-openapi.yml
  format: yaml
  label: H1 Organizations API
  slug: h1-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-organizations-api-openapi.yml
- filename: h1-insights-price-transparency-api-openapi.yml
  format: yaml
  label: H1 Price Transparency API
  slug: h1-insights-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-price-transparency-api-openapi.yml
- filename: h1-insights-providers-api-openapi.yml
  format: yaml
  label: H1 Providers API
  slug: h1-insights-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-providers-api-openapi.yml
- filename: h1-insights-reference-endpoints-api-openapi.yml
  format: yaml
  label: H1 Reference Endpoints API
  slug: h1-insights-reference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-reference-endpoints-api-openapi.yml
- filename: h1-insights-tins-api-openapi.yml
  format: yaml
  label: H1 TI Ns API
  slug: h1-insights-tins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-tins-api-openapi.yml
- filename: h1-insights-virtual-care-platforms-api-openapi.yml
  format: yaml
  label: H1 Virtual Care Platforms API
  slug: h1-insights-virtual-care-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-virtual-care-platforms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: h1.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 20 15:13:57 2026 GMT
  host: h1.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: ribbon.readme.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.ribbonhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: H1 Insights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H1, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: H1
provider_slug: h1-insights
slug: h1-insights-domain-security
source_filename: h1-insights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: h1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 15:13:57 2026 GMT\n  hsts: null\n- host: ribbon.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: null\n- host: api.ribbonhealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: h1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/security/h1-insights-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- healthcare
- provider-data
- provider-directory
- health-insurance
- price-transparency
- eligibility
- care-navigation
- health-plans
- digital-health
- life-sciences
- clinical-trials
- reference-data
---
