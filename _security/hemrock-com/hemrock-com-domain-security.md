---
api_specs:
- filename: hemrock-com-access-api-openapi.yml
  format: yaml
  label: Hemrock Access API
  slug: hemrock-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-access-api-openapi.yml
- filename: hemrock-com-cap-table-api-openapi.yml
  format: yaml
  label: Hemrock Cap Table API
  slug: hemrock-com-cap-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-cap-table-api-openapi.yml
- filename: hemrock-com-compute-api-openapi.yml
  format: yaml
  label: Hemrock Compute API
  slug: hemrock-com-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-compute-api-openapi.yml
- filename: hemrock-com-ecommerce-forecasting-api-openapi.yml
  format: yaml
  label: Hemrock Ecommerce Forecasting API
  slug: hemrock-com-ecommerce-forecasting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-ecommerce-forecasting-api-openapi.yml
- filename: hemrock-com-exit-waterfall-api-openapi.yml
  format: yaml
  label: Hemrock Exit Waterfall API
  slug: hemrock-com-exit-waterfall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-exit-waterfall-api-openapi.yml
- filename: hemrock-com-fund-economics-api-openapi.yml
  format: yaml
  label: Hemrock Fund Economics API
  slug: hemrock-com-fund-economics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-fund-economics-api-openapi.yml
- filename: hemrock-com-models-api-openapi.yml
  format: yaml
  label: Hemrock Models API
  slug: hemrock-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-models-api-openapi.yml
- filename: hemrock-com-results-api-openapi.yml
  format: yaml
  label: Hemrock Results API
  slug: hemrock-com-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-results-api-openapi.yml
- filename: hemrock-com-saas-forecasting-api-openapi.yml
  format: yaml
  label: Hemrock Saas Forecasting API
  slug: hemrock-com-saas-forecasting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-saas-forecasting-api-openapi.yml
- filename: hemrock-com-unit-economics-api-openapi.yml
  format: yaml
  label: Hemrock Unit Economics API
  slug: hemrock-com-unit-economics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-unit-economics-api-openapi.yml
- filename: hemrock-com-usage-api-openapi.yml
  format: yaml
  label: Hemrock Usage API
  slug: hemrock-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hemrock.com
  spf: true
hosts:
- cert_expires: Feb  5 22:09:25 2027 GMT
  host: hemrock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hemrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hemrock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hemrock
provider_slug: hemrock-com
slug: hemrock-com-domain-security
source_filename: hemrock-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hemrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 22:09:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hemrock.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hemrock-com/security/hemrock-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Open Source
- Artificial Intelligence
- Modeling
- Community
- Company
---
