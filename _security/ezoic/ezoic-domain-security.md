---
api_specs:
- filename: ezoic-access-api-openapi.yml
  format: yaml
  label: ezoic Access API
  slug: ezoic-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-access-api-openapi.yml
- filename: ezoic-products-api-openapi.yml
  format: yaml
  label: ezoic Products API
  slug: ezoic-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-products-api-openapi.yml
- filename: ezoic-purchases-api-openapi.yml
  format: yaml
  label: ezoic Purchases API
  slug: ezoic-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-purchases-api-openapi.yml
- filename: ezoic-cdn-api-openapi.yml
  format: yaml
  label: ezoic CDN API
  slug: ezoic-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-cdn-api-openapi.yml
- filename: ezoic-data-api-openapi.yml
  format: yaml
  label: ezoic Data API
  slug: ezoic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-data-api-openapi.yml
- filename: ezoic-filters-api-openapi.yml
  format: yaml
  label: ezoic Filters API
  slug: ezoic-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-filters-api-openapi.yml
- filename: ezoic-reports-api-openapi.yml
  format: yaml
  label: ezoic Reports API
  slug: ezoic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-reports-api-openapi.yml
- filename: ezoic-segments-api-openapi.yml
  format: yaml
  label: ezoic Segments API
  slug: ezoic-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-segments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ezoic.com
  spf: true
hosts:
- cert_expires: Oct 16 12:07:58 2026 GMT
  host: www.ezoic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 07:16:09 2026 GMT
  host: docs.ezoic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api-gateway.ezoic.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ezoic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ezoic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ezoic
provider_slug: ezoic
slug: ezoic-domain-security
source_filename: ezoic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ezoic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.ezoic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:16:09 2026 GMT\n  hsts: false\n- host: api-gateway.ezoic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ezoic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/security/ezoic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Reporting
- Subscription
- Paywalls
- Identity
- CDN
- Caching
- MCP
- Authentication
- Agents
---
