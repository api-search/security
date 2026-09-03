---
api_specs:
- filename: target-inventory-api-openapi.yml
  format: yaml
  label: target Inventory API
  slug: target-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-inventory-api-openapi.yml
- filename: target-orders-api-openapi.yml
  format: yaml
  label: target Orders API
  slug: target-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-orders-api-openapi.yml
- filename: target-products-api-openapi.yml
  format: yaml
  label: target Products API
  slug: target-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-products-api-openapi.yml
- filename: target-search-api-openapi.yml
  format: yaml
  label: target Search API
  slug: target-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-search-api-openapi.yml
- filename: target-status-api-openapi.yml
  format: yaml
  label: target Status API
  slug: target-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-status-api-openapi.yml
- filename: target-stores-api-openapi.yml
  format: yaml
  label: target Stores API
  slug: target-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-stores-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:certificate.management@target.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: target.com
  spf: true
hosts:
- cert_expires: Mar 11 12:56:33 2027 GMT
  host: www.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 15:20:11 2026 GMT
  host: tech.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 15:20:11 2026 GMT
  host: redsky.target.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Target Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Target, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Target
provider_slug: target
slug: target-domain-security
source_filename: target-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 12:56:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tech.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: redsky.target.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 15:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: target.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:certificate.management@target.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/security/target-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- E-Commerce
- Retail
- Product
- Inventory
- Stores
- Order
---
