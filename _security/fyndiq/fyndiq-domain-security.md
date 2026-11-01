---
api_specs:
- filename: fyndiq-articles-api-openapi.yml
  format: yaml
  label: Fyndiq Articles API
  slug: fyndiq-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-articles-api-openapi.yml
- filename: fyndiq-orders-api-openapi.yml
  format: yaml
  label: Fyndiq Orders API
  slug: fyndiq-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-orders-api-openapi.yml
- filename: fyndiq-carrier-codes-api-openapi.yml
  format: yaml
  label: Fyndiq Carrier Codes API
  slug: fyndiq-carrier-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-carrier-codes-api-openapi.yml
- filename: fyndiq-categories-api-openapi.yml
  format: yaml
  label: Fyndiq Categories API
  slug: fyndiq-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-categories-api-openapi.yml
- filename: fyndiq-financial-reports-api-openapi.yml
  format: yaml
  label: Fyndiq Financial Reports API
  slug: fyndiq-financial-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-financial-reports-api-openapi.yml
- filename: fyndiq-health-api-openapi.yml
  format: yaml
  label: Fyndiq Health API
  slug: fyndiq-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-health-api-openapi.yml
- filename: fyndiq-jobs-api-openapi.yml
  format: yaml
  label: Fyndiq Jobs API
  slug: fyndiq-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-jobs-api-openapi.yml
- filename: fyndiq-merchant-api-openapi.yml
  format: yaml
  label: Fyndiq Merchant API
  slug: fyndiq-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-merchant-api-openapi.yml
- filename: fyndiq-sales-funnels-api-openapi.yml
  format: yaml
  label: Fyndiq Sales Funnels API
  slug: fyndiq-sales-funnels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-sales-funnels-api-openapi.yml
- filename: fyndiq-shipping-configurations-api-openapi.yml
  format: yaml
  label: Fyndiq Shipping Configurations API
  slug: fyndiq-shipping-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-shipping-configurations-api-openapi.yml
- filename: fyndiq-statuses-api-openapi.yml
  format: yaml
  label: Fyndiq Statuses API
  slug: fyndiq-statuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fyndiq/openapi/fyndiq-statuses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fyndiq.se
  spf: true
hosts:
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: www.fyndiq.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: merchants-api.fyndiq.se
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: merchants-api.sandbox.fyndiq.se
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fyndiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyndiq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fyndiq
provider_slug: fyndiq
slug: fyndiq-domain-security
source_filename: fyndiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: merchants-api.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: null\n- host: merchants-api.sandbox.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: null\ndomains:\n- domain: fyndiq.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fyndiq/security/fyndiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Marketplace
- E-Commerce
- Retail
- Product
- Order
- Sweden
---
