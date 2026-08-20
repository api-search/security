---
api_specs:
- filename: trend-api-openapi.yml
  format: yaml
  label: Trend API
  slug: trend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trend/refs/heads/main/openapi/trend-api-openapi.yml
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
- User Generated Content
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
