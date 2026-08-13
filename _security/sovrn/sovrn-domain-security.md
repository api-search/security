---
api_specs:
- filename: sovrn-commerce-link-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Link Check API
  slug: sovrn-commerce-link-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-link-check-openapi.yml
- filename: sovrn-commerce-bid-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Bid Check API
  slug: sovrn-commerce-bid-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-bid-check-openapi.yml
- filename: sovrn-commerce-campaigns-openapi.yml
  format: yaml
  label: Sovrn Commerce Campaigns API
  slug: sovrn-commerce-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-campaigns-openapi.yml
- filename: sovrn-commerce-reports-openapi.yml
  format: yaml
  label: Sovrn Commerce Real-Time Reports API
  slug: sovrn-commerce-real-time-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-commerce-reports-openapi.yml
- filename: sovrn-merchant-summaries-openapi.yml
  format: yaml
  label: Sovrn Commerce Merchant Group Summaries API
  slug: sovrn-commerce-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-merchant-summaries-openapi.yml
- filename: sovrn-product-recommendations-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Recommendation API
  slug: sovrn-commerce-product-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-product-recommendations-openapi.yml
- filename: sovrn-price-comparisons-openapi.yml
  format: yaml
  label: Sovrn Commerce Price Comparisons (Product Affiliate) API
  slug: sovrn-commerce-price-comparisons-product-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-price-comparisons-openapi.yml
- filename: sovrn-product-coupons-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Promo Codes API
  slug: sovrn-commerce-product-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-product-coupons-openapi.yml
- filename: sovrn-advertising-reporting-openapi.yml
  format: yaml
  label: Sovrn Advertising Performance Reporting API
  slug: sovrn-advertising-performance-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-advertising-reporting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sovrn.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viglink.com
  spf: true
hosts:
- cert_expires: Oct 18 21:59:55 2026 GMT
  host: www.sovrn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.sovrn.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.viglink.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sovrn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sovrn, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Sovrn
provider_slug: sovrn
slug: sovrn-domain-security
source_filename: sovrn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sovrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:59:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sovrn.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.viglink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sovrn.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: viglink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/security/sovrn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Adtech
- Advertising
- Monetization
- Affiliate Marketing
- Programmatic
- Publishers
- Commerce
- Data
- Reporting
- Product Data
- Agent Native
---
