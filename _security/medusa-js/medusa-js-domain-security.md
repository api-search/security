---
api_specs:
- filename: medusa-js-auth-api-openapi.yml
  format: yaml
  label: Medusa Auth API
  slug: medusa-js-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-auth-api-openapi.yml
- filename: medusa-js-carts-api-openapi.yml
  format: yaml
  label: Medusa Carts API
  slug: medusa-js-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-carts-api-openapi.yml
- filename: medusa-js-categories-api-openapi.yml
  format: yaml
  label: Medusa Categories API
  slug: medusa-js-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-categories-api-openapi.yml
- filename: medusa-js-collections-api-openapi.yml
  format: yaml
  label: Medusa Collections API
  slug: medusa-js-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-collections-api-openapi.yml
- filename: medusa-js-customers-api-openapi.yml
  format: yaml
  label: Medusa Customers API
  slug: medusa-js-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-customers-api-openapi.yml
- filename: medusa-js-orders-api-openapi.yml
  format: yaml
  label: Medusa Orders API
  slug: medusa-js-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-orders-api-openapi.yml
- filename: medusa-js-payments-api-openapi.yml
  format: yaml
  label: Medusa Payments API
  slug: medusa-js-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-payments-api-openapi.yml
- filename: medusa-js-products-api-openapi.yml
  format: yaml
  label: Medusa Products API
  slug: medusa-js-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-products-api-openapi.yml
- filename: medusa-js-regions-api-openapi.yml
  format: yaml
  label: Medusa Regions API
  slug: medusa-js-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-regions-api-openapi.yml
- filename: medusa-js-shipping-api-openapi.yml
  format: yaml
  label: Medusa Shipping API
  slug: medusa-js-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/openapi/medusa-js-shipping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medusajs.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Aug 19 15:01:01 2026 GMT
  host: medusajs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 12:37:45 2026 GMT
  host: docs.medusajs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medusa Js Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medusa, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medusa
provider_slug: medusa-js
slug: medusa-js-domain-security
source_filename: medusa-js-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medusajs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.medusajs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:37:45 2026 GMT\n  hsts: false\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: null\ndomains:\n- domain: medusajs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/security/medusa-js-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commerce
- Headless
- eCommerce
- Open Source
- Node.js
- TypeScript
- Framework
- Modules
- Workflows
- MCP
---
