---
api_specs:
- filename: lycatra-com-cart-api-openapi.yml
  format: yaml
  label: Lycatra Cart API
  slug: lycatra-com-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-cart-api-openapi.yml
- filename: lycatra-com-carts-api-openapi.yml
  format: yaml
  label: Lycatra Carts API
  slug: lycatra-com-carts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-carts-api-openapi.yml
- filename: lycatra-com-categories-api-openapi.yml
  format: yaml
  label: Lycatra Categories API
  slug: lycatra-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-categories-api-openapi.yml
- filename: lycatra-com-products-api-openapi.yml
  format: yaml
  label: Lycatra Products API
  slug: lycatra-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-products-api-openapi.yml
- filename: lycatra-com-requests-api-openapi.yml
  format: yaml
  label: Lycatra Requests API
  slug: lycatra-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-requests-api-openapi.yml
- filename: lycatra-com-shops-api-openapi.yml
  format: yaml
  label: Lycatra Shops API
  slug: lycatra-com-shops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lycatra-com/openapi/lycatra-com-shops-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lycatra.com
  spf: true
hosts:
- cert_expires: Jan  2 02:14:19 2027 GMT
  host: lycatra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lycatra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lycatra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lycatra
provider_slug: lycatra-com
slug: lycatra-com-domain-security
source_filename: lycatra-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lycatra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 02:14:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lycatra.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lycatra-com/security/lycatra-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Film
- Rentals
- Equipment
- Swiss
---
