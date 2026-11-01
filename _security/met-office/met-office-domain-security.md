---
api_specs:
- filename: met-office-capabilities-api-openapi.yml
  format: yaml
  label: Met Office Capabilities API
  slug: met-office-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-capabilities-api-openapi.yml
- filename: met-office-collection-metadata-api-openapi.yml
  format: yaml
  label: Met Office Collection Metadata API
  slug: met-office-collection-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-collection-metadata-api-openapi.yml
- filename: met-office-instance-data-api-openapi.yml
  format: yaml
  label: Met Office Instance Data API
  slug: met-office-instance-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-data-api-openapi.yml
- filename: met-office-instance-metadata-api-openapi.yml
  format: yaml
  label: Met Office Instance Metadata API
  slug: met-office-instance-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-instance-metadata-api-openapi.yml
- filename: met-office-met-office-land-observations-public-api-api-openapi.yml
  format: yaml
  label: Met Office Met Office Land Observations Public API
  slug: met-office-met-office-land-observations-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-met-office-land-observations-public-api-api-openapi.yml
- filename: met-office-nearest-api-openapi.yml
  format: yaml
  label: Met Office Nearest API
  slug: met-office-nearest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-nearest-api-openapi.yml
- filename: met-office-objects-api-openapi.yml
  format: yaml
  label: Met Office Objects API
  slug: met-office-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-objects-api-openapi.yml
- filename: met-office-orders-api-openapi.yml
  format: yaml
  label: Met Office Orders API
  slug: met-office-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-orders-api-openapi.yml
- filename: met-office-point-api-openapi.yml
  format: yaml
  label: Met Office Point API
  slug: met-office-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-point-api-openapi.yml
- filename: met-office-runs-api-openapi.yml
  format: yaml
  label: Met Office Runs API
  slug: met-office-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/met-office/openapi/met-office-runs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metoffice.gov.uk
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: metoffice.gov.uk
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Met Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Met Office, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Met Office
provider_slug: met-office
slug: met-office-domain-security
source_filename: met-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metoffice.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: metoffice.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/met-office/security/met-office-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather
- Climate
- Forecast
- Meteorology
- Government
- Open Data
- United Kingdom
---
