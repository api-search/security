---
api_specs:
- filename: sovrn-account-api-openapi.yml
  format: yaml
  label: Sovrn Account API
  slug: sovrn-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-account-api-openapi.yml
- filename: sovrn-ai-orchestration-api-openapi.yml
  format: yaml
  label: Sovrn Ai Orchestration API
  slug: sovrn-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-ai-orchestration-api-openapi.yml
- filename: sovrn-bid-api-openapi.yml
  format: yaml
  label: Sovrn Bid API
  slug: sovrn-bid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-bid-api-openapi.yml
- filename: sovrn-link-api-openapi.yml
  format: yaml
  label: Sovrn Link API
  slug: sovrn-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-link-api-openapi.yml
- filename: sovrn-merchant-group-summaries-api-openapi.yml
  format: yaml
  label: Sovrn Merchant Group Summaries API
  slug: sovrn-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-merchant-group-summaries-api-openapi.yml
- filename: sovrn-product-coupons-api-openapi.yml
  format: yaml
  label: Sovrn Product Coupons API
  slug: sovrn-product-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-product-coupons-api-openapi.yml
- filename: sovrn-reporting-api-openapi.yml
  format: yaml
  label: Sovrn Reporting API
  slug: sovrn-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-reporting-api-openapi.yml
- filename: sovrn-reports-api-openapi.yml
  format: yaml
  label: Sovrn Reports API
  slug: sovrn-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-reports-api-openapi.yml
- filename: sovrn-sites-api-openapi.yml
  format: yaml
  label: Sovrn Sites API
  slug: sovrn-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovrn/refs/heads/main/openapi/sovrn-sites-api-openapi.yml
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
- AdTech
- Advertising
- Monetization
- Affiliate Marketing
- Programmatic
- Publishers
- Commerce
- Data
- Reporting
- Product Data
- agent-native
---
