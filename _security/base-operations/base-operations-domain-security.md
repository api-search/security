---
api_specs:
- filename: base-operations-analytics-api-openapi.yml
  format: yaml
  label: Base Operations Analytics API
  slug: base-operations-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-analytics-api-openapi.yml
- filename: base-operations-base-score-api-openapi.yml
  format: yaml
  label: Base Operations Base Score API
  slug: base-operations-base-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-base-score-api-openapi.yml
- filename: base-operations-change-detection-api-openapi.yml
  format: yaml
  label: Base Operations Change Detection API
  slug: base-operations-change-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-change-detection-api-openapi.yml
- filename: base-operations-key-takeaways-api-openapi.yml
  format: yaml
  label: Base Operations Key Takeaways API
  slug: base-operations-key-takeaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-key-takeaways-api-openapi.yml
- filename: base-operations-public-charts-api-openapi.yml
  format: yaml
  label: Base Operations Public Charts API
  slug: base-operations-public-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-public-charts-api-openapi.yml
- filename: base-operations-radius-charts-api-openapi.yml
  format: yaml
  label: Base Operations Radius Charts API
  slug: base-operations-radius-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-radius-charts-api-openapi.yml
- filename: base-operations-saved-location-charts-api-openapi.yml
  format: yaml
  label: Base Operations Saved Location Charts API
  slug: base-operations-saved-location-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-location-charts-api-openapi.yml
- filename: base-operations-saved-location-radius-charts-api-openapi.yml
  format: yaml
  label: Base Operations Saved Location Radius Charts API
  slug: base-operations-saved-location-radius-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-location-radius-charts-api-openapi.yml
- filename: base-operations-saved-locations-api-openapi.yml
  format: yaml
  label: Base Operations Saved Locations API
  slug: base-operations-saved-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-saved-locations-api-openapi.yml
- filename: base-operations-source-categories-api-openapi.yml
  format: yaml
  label: Base Operations Source Categories API
  slug: base-operations-source-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-source-categories-api-openapi.yml
- filename: base-operations-threat-categories-api-openapi.yml
  format: yaml
  label: Base Operations Threat Categories API
  slug: base-operations-threat-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-threat-categories-api-openapi.yml
- filename: base-operations-threats-api-openapi.yml
  format: yaml
  label: Base Operations Threats API
  slug: base-operations-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/openapi/base-operations-threats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baseoperations.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: baseoperationsenterprise.com
  spf: false
hosts:
- cert_expires: Sep 11 05:01:36 2026 GMT
  host: www.baseoperations.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.baseoperationsenterprise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base Operations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base Operations, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Base Operations
provider_slug: base-operations
slug: base-operations-domain-security
source_filename: base-operations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baseoperations.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:01:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.baseoperationsenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baseoperations.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: baseoperationsenterprise.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-operations/refs/heads/main/security/base-operations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Threat Intelligence
- Security
- Risk Management
- Physical Security
- Crime Data
- Geospatial
- Public Safety
- Risk Scoring
---
