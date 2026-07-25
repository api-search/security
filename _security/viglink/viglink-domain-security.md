---
api_specs:
- filename: viglink-account-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Account API
  slug: viglink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-account-api-openapi.yml
- filename: viglink-ai-orchestration-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Ai Orchestration API
  slug: viglink-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-ai-orchestration-api-openapi.yml
- filename: viglink-bid-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Bid API
  slug: viglink-bid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-api-openapi.yml
- filename: viglink-link-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Link API
  slug: viglink-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-api-openapi.yml
- filename: viglink-merchant-group-summaries-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Merchant Group Summaries API
  slug: viglink-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-group-summaries-api-openapi.yml
- filename: viglink-product-coupons-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Product Coupons API
  slug: viglink-product-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-coupons-api-openapi.yml
- filename: viglink-reports-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) reports API
  slug: viglink-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-api-openapi.yml
- filename: viglink-sites-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Sites API
  slug: viglink-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-sites-api-openapi.yml
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
