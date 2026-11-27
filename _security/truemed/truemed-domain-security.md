---
api_specs:
- filename: truemed-disputes-api-openapi.yml
  format: yaml
  label: Truemed Disputes API
  slug: truemed-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-disputes-api-openapi.yml
- filename: truemed-eligibility-api-openapi.yml
  format: yaml
  label: Truemed Eligibility API
  slug: truemed-eligibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-eligibility-api-openapi.yml
- filename: truemed-files-api-openapi.yml
  format: yaml
  label: Truemed Files API
  slug: truemed-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-files-api-openapi.yml
- filename: truemed-paymentsessions-api-openapi.yml
  format: yaml
  label: Truemed Payment Sessions API
  slug: truemed-paymentsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-paymentsessions-api-openapi.yml
- filename: truemed-paymenttokens-api-openapi.yml
  format: yaml
  label: Truemed Payment Tokens API
  slug: truemed-paymenttokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-paymenttokens-api-openapi.yml
- filename: truemed-qualificationsessions-api-openapi.yml
  format: yaml
  label: Truemed Qualification Sessions API
  slug: truemed-qualificationsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-qualificationsessions-api-openapi.yml
- filename: truemed-reconciliations-api-openapi.yml
  format: yaml
  label: Truemed Reconciliations API
  slug: truemed-reconciliations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-reconciliations-api-openapi.yml
- filename: truemed-product-catalog-api-openapi.yml
  format: yaml
  label: Truemed Product Catalog API
  slug: truemed-product-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truemed/openapi/truemed-product-catalog-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: truemed.com
  spf: true
hosts:
- cert_expires: Jan 23 01:49:43 2027 GMT
  host: truemed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Truemed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truemed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Truemed
provider_slug: truemed
slug: truemed-domain-security
source_filename: truemed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truemed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 01:49:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: truemed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/truemed/security/truemed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Fintech
- HSA
- FSA
- Payments
---
