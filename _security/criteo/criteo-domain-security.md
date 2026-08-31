---
api_specs:
- filename: criteo-accounts-api-openapi.yml
  format: yaml
  label: Criteo Accounts API
  slug: criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-accounts-api-openapi.yml
- filename: criteo-advertiser-api-openapi.yml
  format: yaml
  label: Criteo Advertiser API
  slug: criteo-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-advertiser-api-openapi.yml
- filename: criteo-analytics-api-openapi.yml
  format: yaml
  label: Criteo Analytics API
  slug: criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-analytics-api-openapi.yml
- filename: criteo-audience-api-openapi.yml
  format: yaml
  label: Criteo Audience API
  slug: criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-audience-api-openapi.yml
- filename: criteo-balance-api-openapi.yml
  format: yaml
  label: Criteo Balance API
  slug: criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-balance-api-openapi.yml
- filename: criteo-billing-api-openapi.yml
  format: yaml
  label: Criteo Billing API
  slug: criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-billing-api-openapi.yml
- filename: criteo-campaign-api-openapi.yml
  format: yaml
  label: Criteo Campaign API
  slug: criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-campaign-api-openapi.yml
- filename: criteo-catalog-api-openapi.yml
  format: yaml
  label: Criteo Catalog API
  slug: criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-catalog-api-openapi.yml
- filename: criteo-creative-api-openapi.yml
  format: yaml
  label: Criteo Creative API
  slug: criteo-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-creative-api-openapi.yml
- filename: criteo-gateway-api-openapi.yml
  format: yaml
  label: Criteo Gateway API
  slug: criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-gateway-api-openapi.yml
- filename: criteo-reco-api-openapi.yml
  format: yaml
  label: Criteo Reco API
  slug: criteo-reco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-reco-api-openapi.yml
- filename: criteo-segment-api-openapi.yml
  format: yaml
  label: Criteo Segment API
  slug: criteo-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/openapi/criteo-segment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: criteo.com
  spf: true
hosts:
- cert_expires: Sep 14 13:49:57 2026 GMT
  host: www.criteo.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:16:40 2026 GMT
  host: developers.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.criteo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Criteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Criteo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Criteo
provider_slug: criteo
slug: criteo-domain-security
source_filename: criteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:16:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.criteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: criteo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/criteo/refs/heads/main/security/criteo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Agent Skills
- Analytics
- Audiences
- Campaigns
- Catalog
- Commerce
- Commerce Media
- Display Advertising
- Marketing
- MCP
- Media
- Authentication
- OpenAPI
- Reporting
- Retail
- Retail Media
- Sponsored Products
---
