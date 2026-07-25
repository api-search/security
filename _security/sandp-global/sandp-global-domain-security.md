---
api_specs:
- filename: sandp-global-authentication-api-openapi.yml
  format: yaml
  label: S&P Global Authentication API
  slug: sandp-global-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-authentication-api-openapi.yml
- filename: sandp-global-financial-data-api-openapi.yml
  format: yaml
  label: S&P Global Financial Data API
  slug: sandp-global-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-financial-data-api-openapi.yml
- filename: sandp-global-market-data-api-openapi.yml
  format: yaml
  label: S&P Global Market Data API
  slug: sandp-global-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-market-data-api-openapi.yml
- filename: sandp-global-price-assessments-api-openapi.yml
  format: yaml
  label: S&P Global Price Assessments API
  slug: sandp-global-price-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-price-assessments-api-openapi.yml
- filename: sandp-global-reference-data-api-openapi.yml
  format: yaml
  label: S&P Global Reference Data API
  slug: sandp-global-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/openapi/sandp-global-reference-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spglobal.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.spglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.marketplace.spglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: developer.spglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sandp Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for S&P Global, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: S&P Global
provider_slug: sandp-global
slug: sandp-global-domain-security
source_filename: sandp-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: www.marketplace.spglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.spglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: spglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandp-global/refs/heads/main/security/sandp-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Market Intelligence
- Commodity Insights
- Credit Ratings
- Analytics
- Fortune 500
- Enterprise
---
