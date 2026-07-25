---
api_specs:
- filename: shopware-account-api-openapi.yml
  format: yaml
  label: Shopware Account API
  slug: shopware-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-account-api-openapi.yml
- filename: shopware-bulk-api-openapi.yml
  format: yaml
  label: Shopware Bulk API
  slug: shopware-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-bulk-api-openapi.yml
- filename: shopware-cart-api-openapi.yml
  format: yaml
  label: Shopware Cart API
  slug: shopware-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-cart-api-openapi.yml
- filename: shopware-category-api-openapi.yml
  format: yaml
  label: Shopware Category API
  slug: shopware-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-category-api-openapi.yml
- filename: shopware-checkout-api-openapi.yml
  format: yaml
  label: Shopware Checkout API
  slug: shopware-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-checkout-api-openapi.yml
- filename: shopware-customer-api-openapi.yml
  format: yaml
  label: Shopware Customer API
  slug: shopware-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-customer-api-openapi.yml
- filename: shopware-navigation-api-openapi.yml
  format: yaml
  label: Shopware Navigation API
  slug: shopware-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-navigation-api-openapi.yml
- filename: shopware-order-api-openapi.yml
  format: yaml
  label: Shopware Order API
  slug: shopware-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-order-api-openapi.yml
- filename: shopware-product-api-openapi.yml
  format: yaml
  label: Shopware Product API
  slug: shopware-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-product-api-openapi.yml
- filename: shopware-search-api-openapi.yml
  format: yaml
  label: Shopware Search API
  slug: shopware-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shopware.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.shopware.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: shopware.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopware, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shopware
provider_slug: shopware
slug: shopware-domain-security
source_filename: shopware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shopware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: shopware.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shopware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/security/shopware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Open Source
- Headless Commerce
- B2B
- B2C
- REST
- OAuth2
---
