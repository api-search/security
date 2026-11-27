---
api_specs:
- filename: propertyindex-ae-account-api-openapi.yml
  format: yaml
  label: PropertyIndex Account API
  slug: propertyindex-ae-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propertyindex-ae/openapi/propertyindex-ae-account-api-openapi.yml
- filename: propertyindex-ae-locations-api-openapi.yml
  format: yaml
  label: PropertyIndex Locations API
  slug: propertyindex-ae-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propertyindex-ae/openapi/propertyindex-ae-locations-api-openapi.yml
- filename: propertyindex-ae-market-index-api-openapi.yml
  format: yaml
  label: PropertyIndex Market index API
  slug: propertyindex-ae-market-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propertyindex-ae/openapi/propertyindex-ae-market-index-api-openapi.yml
- filename: propertyindex-ae-rentals-api-openapi.yml
  format: yaml
  label: PropertyIndex Rentals API
  slug: propertyindex-ae-rentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propertyindex-ae/openapi/propertyindex-ae-rentals-api-openapi.yml
- filename: propertyindex-ae-sales-api-openapi.yml
  format: yaml
  label: PropertyIndex Sales API
  slug: propertyindex-ae-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propertyindex-ae/openapi/propertyindex-ae-sales-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: propertyindex.ae
  spf: false
hosts:
- cert_expires: Dec 30 16:06:33 2026 GMT
  host: www.propertyindex.ae
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PropertyIndex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PropertyIndex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: PropertyIndex
provider_slug: propertyindex-ae
slug: propertyindex-ae-domain-security
source_filename: propertyindex-ae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propertyindex.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 16:06:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: propertyindex.ae\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/propertyindex-ae/security/propertyindex-ae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Dubai
- Property Data
- Market Intelligence
---
