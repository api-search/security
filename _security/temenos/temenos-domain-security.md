---
api_specs:
- filename: openapi.json
  format: json
  label: Temenos Transact API
  slug: temenos-transact-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/transact/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Infinity API
  slug: temenos-infinity-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/infinity/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Payments API
  slug: temenos-payments-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/payments/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Fund Administration API
  slug: temenos-fund-administration-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/funds/openapi.json
- filename: openapi.json
  format: json
  label: Temenos Financial Crime Mitigation API
  slug: temenos-financial-crime-mitigation-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/fcm/openapi.json
- filename: temenos-data-hub-openapi.yml
  format: yaml
  label: Temenos Transact Data Hub API
  slug: temenos-transact-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-data-hub-openapi.yml
- filename: temenos-wealth-openapi.yml
  format: yaml
  label: Temenos Wealth API
  slug: temenos-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-wealth-openapi.yml
- filename: temenos-enterprise-product-pricing-openapi.yml
  format: yaml
  label: Temenos Enterprise Product and Pricing API
  slug: temenos-enterprise-product-and-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-enterprise-product-pricing-openapi.yml
- filename: temenos-cloud-banking-openapi.yml
  format: yaml
  label: Temenos Cloud Banking (CMB) API
  slug: temenos-cloud-banking-cmb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-cloud-banking-openapi.yml
- filename: temenos-journey-manager-openapi.yml
  format: yaml
  label: Temenos Journey Manager API
  slug: temenos-journey-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-journey-manager-openapi.yml
- filename: temenos-microservices-openapi.yml
  format: yaml
  label: Temenos Transact Microservices API
  slug: temenos-transact-microservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-microservices-openapi.yml
- filename: temenos-bnpl-openapi.yml
  format: yaml
  label: Temenos Buy Now Pay Later API
  slug: temenos-buy-now-pay-later-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/openapi/temenos-bnpl-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: temenos.com
  spf: true
hosts:
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: apidocs.temenos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: www.temenos.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 14 23:59:59 2026 GMT
  host: api.temenos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Temenos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temenos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temenos
provider_slug: temenos
slug: temenos-domain-security
source_filename: temenos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidocs.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: false\n- host: api.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: temenos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/security/temenos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
---
