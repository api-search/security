---
api_specs:
- filename: trend-ai-api-openapi.yml
  format: yaml
  label: Trend AI API
  slug: trend-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-ai-api-openapi.yml
- filename: trend-auth-api-openapi.yml
  format: yaml
  label: Trend Auth API
  slug: trend-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-auth-api-openapi.yml
- filename: trend-basic-authentication-ai-api-openapi.yml
  format: yaml
  label: Trend Basic Authentication (AI) API
  slug: trend-basic-authentication-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-basic-authentication-ai-api-openapi.yml
- filename: trend-brand-admin-api-openapi.yml
  format: yaml
  label: Trend Brand Admin API
  slug: trend-brand-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-admin-api-openapi.yml
- filename: trend-brand-api-openapi.yml
  format: yaml
  label: Trend Brand API
  slug: trend-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-api-openapi.yml
- filename: trend-brand-authentication-api-openapi.yml
  format: yaml
  label: Trend Brand Authentication API
  slug: trend-brand-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-brand-authentication-api-openapi.yml
- filename: trend-campaign-api-openapi.yml
  format: yaml
  label: Trend Campaign API
  slug: trend-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-campaign-api-openapi.yml
- filename: trend-content-api-openapi.yml
  format: yaml
  label: Trend Content API
  slug: trend-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-content-api-openapi.yml
- filename: trend-creator-api-openapi.yml
  format: yaml
  label: Trend Creator API
  slug: trend-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-api-openapi.yml
- filename: trend-creator-authentication-api-openapi.yml
  format: yaml
  label: Trend Creator Authentication API
  slug: trend-creator-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-authentication-api-openapi.yml
- filename: trend-creator-portfolio-api-openapi.yml
  format: yaml
  label: Trend Creator Portfolio API
  slug: trend-creator-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-portfolio-api-openapi.yml
- filename: trend-creator-profiles-api-openapi.yml
  format: yaml
  label: Trend Creator Profiles API
  slug: trend-creator-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-creator-profiles-api-openapi.yml
- filename: trend-health-check-api-openapi.yml
  format: yaml
  label: Trend Health Check API
  slug: trend-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-health-check-api-openapi.yml
- filename: trend-message-api-openapi.yml
  format: yaml
  label: Trend Message API
  slug: trend-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-message-api-openapi.yml
- filename: trend-metrics-api-openapi.yml
  format: yaml
  label: Trend Metrics API
  slug: trend-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-metrics-api-openapi.yml
- filename: trend-partnership-api-openapi.yml
  format: yaml
  label: Trend Partnership API
  slug: trend-partnership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-partnership-api-openapi.yml
- filename: trend-payment-api-openapi.yml
  format: yaml
  label: Trend Payment API
  slug: trend-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-payment-api-openapi.yml
- filename: trend-review-api-openapi.yml
  format: yaml
  label: Trend Review API
  slug: trend-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-review-api-openapi.yml
- filename: trend-shipment-api-openapi.yml
  format: yaml
  label: Trend Shipment API
  slug: trend-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-shipment-api-openapi.yml
- filename: trend-upload-api-openapi.yml
  format: yaml
  label: Trend Upload API
  slug: trend-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-upload-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trend.io
  spf: true
hosts:
- cert_expires: Oct 15 02:02:36 2026 GMT
  host: trend.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.trend.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trend
provider_slug: trend
slug: trend-domain-security
source_filename: trend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trend.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: trend.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/security/trend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- User-Generated Content
- Creator Economy
- Content Marketing
- Video Production
- Photography
- Marketing
- E-Commerce
- Creator Marketplace
- Influencer Marketing
- AI Image Generation
- Payments
---
