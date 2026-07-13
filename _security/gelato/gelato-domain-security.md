---
api_specs:
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Orders API
  slug: gelato-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Product Catalog API
  slug: gelato-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Prices and Stock API
  slug: gelato-prices-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Shipment API
  slug: gelato-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Ecommerce API
  slug: gelato-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
- filename: gelato-openapi.yml
  format: yaml
  label: Gelato Webhooks API
  slug: gelato-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/openapi/gelato-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gelato.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gelatoapis.com
  spf: false
hosts:
- cert_expires: Sep 29 17:57:51 2026 GMT
  host: www.gelato.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:44:52 2026 GMT
  host: dashboard.gelato.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 03:50:46 2026 GMT
  host: order.gelatoapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gelato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gelato, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gelato
provider_slug: gelato
slug: gelato-domain-security
source_filename: gelato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gelato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: dashboard.gelato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:44:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: order.gelatoapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:50:46 2026 GMT\n  hsts: null\ndomains:\n- domain: gelato.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gelatoapis.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n \
  \ - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gelato/refs/heads/main/security/gelato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Print on Demand
- Ecommerce
- Fulfillment
- Distributed Production
- Orders
---
