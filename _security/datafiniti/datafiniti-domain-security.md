---
api_specs:
- filename: datafiniti-properties-api-openapi.yml
  format: yaml
  label: Datafiniti Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-properties-api-openapi.yml
- filename: datafiniti-people-api-openapi.yml
  format: yaml
  label: Datafiniti People Data API
  slug: people-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-people-api-openapi.yml
- filename: datafiniti-businesses-api-openapi.yml
  format: yaml
  label: Datafiniti Business Data API
  slug: business-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-businesses-api-openapi.yml
- filename: datafiniti-products-api-openapi.yml
  format: yaml
  label: Datafiniti Product Data API
  slug: product-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-products-api-openapi.yml
- filename: datafiniti-downloads-api-openapi.yml
  format: yaml
  label: Datafiniti Downloads API
  slug: downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-downloads-api-openapi.yml
- filename: datafiniti-views-api-openapi.yml
  format: yaml
  label: Datafiniti Views API
  slug: views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-views-api-openapi.yml
- filename: datafiniti-real-time-data-requests-api-openapi.yml
  format: yaml
  label: Datafiniti Real-time Data Requests API
  slug: real-time-data-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-real-time-data-requests-api-openapi.yml
- filename: datafiniti-authentication-api-openapi.yml
  format: yaml
  label: Datafiniti Authentication API
  slug: datafiniti-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-authentication-api-openapi.yml
- filename: datafiniti-account-api-openapi.yml
  format: yaml
  label: Datafiniti Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-account-api-openapi.yml
- filename: datafiniti-status-api-openapi.yml
  format: yaml
  label: Datafiniti Status API
  slug: status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datafiniti.co
  spf: true
hosts:
- cert_expires: Aug 16 07:01:49 2026 GMT
  host: www.datafiniti.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:32:00 2026 GMT
  host: docs.datafiniti.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.datafiniti.co
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Datafiniti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datafiniti, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datafiniti
provider_slug: datafiniti
slug: datafiniti-domain-security
source_filename: datafiniti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datafiniti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.datafiniti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.datafiniti.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datafiniti.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datafiniti/security/datafiniti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Data
- Data Aggregation
- Data as a Service
- Data Enrichment
- MCP
- People Data
- Product Data
- Property Data
- Real Estate
---
