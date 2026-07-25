---
api_specs:
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Providers API
  slug: ribbon-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Locations API
  slug: ribbon-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Custom Filters API
  slug: ribbon-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Focus Areas API
  slug: ribbon-focus-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Price Transparency API
  slug: ribbon-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Cost Estimates & Eligibility API
  slug: ribbon-cost-estimates-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Organizations API
  slug: ribbon-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Reference Data API
  slug: ribbon-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
- filename: ribbon-health-api-openapi.json
  format: json
  label: H1 Ribbon Network Analysis API
  slug: ribbon-network-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/openapi/ribbon-health-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: h1.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 13 08:52:44 2026 GMT
  host: h1.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: ribbon.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.ribbonhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: H1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H1, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: H1
provider_slug: h1
slug: h1-domain-security
source_filename: h1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: h1.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:52:44 2026 GMT\n  hsts: false\n- host: ribbon.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ribbonhealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: h1.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h1/refs/heads/main/security/h1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Life Sciences
- Provider Data
- Healthcare API
- Price Transparency
- Eligibility
- Network Intelligence
- Digital Health
- Pharma
---
