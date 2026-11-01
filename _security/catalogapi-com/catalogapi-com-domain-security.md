---
api_specs:
- filename: catalogapi-com-cart-api-openapi.yml
  format: yaml
  label: catalogapi-com Cart API
  slug: catalogapi-com-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-cart-api-openapi.yml
- filename: catalogapi-com-catalog-api-openapi.yml
  format: yaml
  label: catalogapi-com Catalog API
  slug: catalogapi-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-catalog-api-openapi.yml
- filename: catalogapi-com-health-api-openapi.yml
  format: yaml
  label: catalogapi-com Health API
  slug: catalogapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-health-api-openapi.yml
- filename: catalogapi-com-order-api-openapi.yml
  format: yaml
  label: catalogapi-com Order API
  slug: catalogapi-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-order-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catalogapi.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: catalogapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catalogapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for catalogapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: catalogapi-com
provider_slug: catalogapi-com
slug: catalogapi-com-domain-security
source_filename: catalogapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalogapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: catalogapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/catalogapi-com/security/catalogapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Rewards
- GiftCards
- Global
---
