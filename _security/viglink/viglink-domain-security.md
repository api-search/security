---
api_specs:
- filename: viglink-link-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Link Check API
  slug: link-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-check-openapi.yml
- filename: viglink-bid-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Bid Check API
  slug: bid-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-check-openapi.yml
- filename: viglink-campaigns-openapi.yml
  format: yaml
  label: Sovrn Commerce Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-campaigns-openapi.yml
- filename: viglink-reports-openapi.yml
  format: yaml
  label: Sovrn Commerce Real-Time Reports API
  slug: real-time-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-openapi.yml
- filename: viglink-merchant-summaries-openapi.yml
  format: yaml
  label: Sovrn Commerce Merchant Group Summaries API
  slug: merchant-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-summaries-openapi.yml
- filename: viglink-product-recommendations-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Recommendations API
  slug: product-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-recommendations-openapi.yml
- filename: viglink-product-promo-codes-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Promo Codes API
  slug: product-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-promo-codes-openapi.yml
- filename: viglink-price-comparisons-openapi.yml
  format: yaml
  label: Sovrn Commerce Price Comparisons API
  slug: price-comparisons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-price-comparisons-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sovrn.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viglink.com
  spf: true
hosts:
- cert_expires: Oct 18 21:59:55 2026 GMT
  host: sovrn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:45:33 2026 GMT
  host: developer.sovrn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.viglink.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Viglink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VigLink (Sovrn Commerce), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VigLink (Sovrn Commerce)
provider_slug: viglink
slug: viglink-domain-security
source_filename: viglink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sovrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:59:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.sovrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:45:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.viglink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sovrn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: viglink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/security/viglink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Commerce
- Monetization
- Publishers
- Links
- Advertising
- Reporting
---
