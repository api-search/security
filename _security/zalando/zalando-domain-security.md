---
api_specs:
- filename: zalando-orders-openapi.yml
  format: yaml
  label: zDirect Platform Orders API
  slug: zalando-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-orders-openapi.yml
- filename: zalando-products-openapi.yml
  format: yaml
  label: zDirect Platform Products API
  slug: zalando-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-products-openapi.yml
- filename: zalando-product-attributes-openapi.yml
  format: yaml
  label: Merchant Product Attributes API
  slug: zalando-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-product-attributes-openapi.yml
- filename: zalando-article-requirements-openapi.yml
  format: yaml
  label: Article Requirements API
  slug: zalando-article-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-article-requirements-openapi.yml
- filename: zalando-prices-openapi.yml
  format: yaml
  label: Merchant Price Service API
  slug: zalando-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-prices-openapi.yml
- filename: zalando-price-reporting-openapi.yml
  format: yaml
  label: Price Reporting API
  slug: zalando-price-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-price-reporting-openapi.yml
- filename: zalando-stocks-openapi.yml
  format: yaml
  label: Merchant Stock Service API
  slug: zalando-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-stocks-openapi.yml
- filename: zalando-offer-blocking-openapi.yml
  format: yaml
  label: Article Availability (Offer Blocking) API
  slug: zalando-offer-blocking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-offer-blocking-openapi.yml
- filename: zalando-sales-channels-openapi.yml
  format: yaml
  label: Sales Channels API
  slug: zalando-sales-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-sales-channels-openapi.yml
- filename: zalando-logistic-centers-openapi.yml
  format: yaml
  label: Logistic Centers API
  slug: zalando-logistic-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-logistic-centers-openapi.yml
- filename: zalando-zfs-stock-movements-openapi.yml
  format: yaml
  label: ZFS Stock Movements API
  slug: zalando-zfs-stock-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-stock-movements-openapi.yml
- filename: zalando-zfs-cross-border-movements-openapi.yml
  format: yaml
  label: ZFS Cross-Border Movements Report API
  slug: zalando-zfs-cross-border-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-cross-border-movements-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zalando.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: corporate.zalando.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: developers.merchants.zalando.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.merchants.zalando.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zalando Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zalando, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zalando
provider_slug: zalando
slug: zalando-domain-security
source_filename: zalando-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: developers.merchants.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.merchants.zalando.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zalando.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/security/zalando-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer; Marketplace
- Fashion
- E-Commerce
- Retail
- Marketplace
- Fulfillment
- Merchant Platform
- Orders
- Products
---
