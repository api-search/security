---
api_specs:
- filename: homecastr-com-auth-api-openapi.yml
  format: yaml
  label: Homecastr Auth API
  slug: homecastr-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-auth-api-openapi.yml
- filename: homecastr-com-benchmarks-api-openapi.yml
  format: yaml
  label: Homecastr Benchmarks API
  slug: homecastr-com-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-benchmarks-api-openapi.yml
- filename: homecastr-com-data-api-openapi.yml
  format: yaml
  label: Homecastr Data API
  slug: homecastr-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-data-api-openapi.yml
- filename: homecastr-com-data-readiness-api-openapi.yml
  format: yaml
  label: Homecastr Data Readiness API
  slug: homecastr-com-data-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-data-readiness-api-openapi.yml
- filename: homecastr-com-forecasts-api-openapi.yml
  format: yaml
  label: Homecastr Forecasts API
  slug: homecastr-com-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-forecasts-api-openapi.yml
- filename: homecastr-com-internal-api-openapi.yml
  format: yaml
  label: Homecastr Internal API
  slug: homecastr-com-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-internal-api-openapi.yml
- filename: homecastr-com-meta-api-openapi.yml
  format: yaml
  label: Homecastr Meta API
  slug: homecastr-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-meta-api-openapi.yml
- filename: homecastr-com-permit-and-zoning-data-api-openapi.yml
  format: yaml
  label: Homecastr Permit and zoning data API
  slug: homecastr-com-permit-and-zoning-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecastr-com/openapi/homecastr-com-permit-and-zoning-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: homecastr.com
  spf: true
hosts:
- cert_expires: Feb  9 18:18:03 2027 GMT
  host: homecastr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homecastr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homecastr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Homecastr
provider_slug: homecastr-com
slug: homecastr-com-domain-security
source_filename: homecastr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homecastr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 18:18:03 2027 GMT\n  hsts: false\ndomains:\n- domain: homecastr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/homecastr-com/security/homecastr-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Data
- Forecasting
- Artificial Intelligence
- Homecastr
---
