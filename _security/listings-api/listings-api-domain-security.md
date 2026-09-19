---
api_specs:
- filename: listings-api-analytics-api-openapi.yml
  format: yaml
  label: Listings API Analytics API
  slug: listings-api-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-analytics-api-openapi.yml
- filename: listings-api-connected-accounts-api-openapi.yml
  format: yaml
  label: Listings API Connected Accounts API
  slug: listings-api-connected-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-connected-accounts-api-openapi.yml
- filename: listings-api-listings-api-openapi.yml
  format: yaml
  label: Listings API Listings API
  slug: listings-api-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-listings-api-openapi.yml
- filename: listings-api-locations-api-openapi.yml
  format: yaml
  label: Listings API Locations API
  slug: listings-api-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-locations-api-openapi.yml
- filename: listings-api-posts-api-openapi.yml
  format: yaml
  label: Listings API Posts API
  slug: listings-api-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-posts-api-openapi.yml
- filename: listings-api-reviews-api-openapi.yml
  format: yaml
  label: Listings API Reviews API
  slug: listings-api-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-reviews-api-openapi.yml
- filename: listings-api-supporting-apis-api-openapi.yml
  format: yaml
  label: Listings API Supporting APIs API
  slug: listings-api-supporting-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/openapi/listings-api-supporting-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listingsapi.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: docs.listingsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: listingsapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Listings Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listings API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Listings API
provider_slug: listings-api
slug: listings-api-domain-security
source_filename: listings-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.listingsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: listingsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: listingsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listings-api/refs/heads/main/security/listings-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Listings
- Local SEO
- Location
- Reviews
- Google Business Profile
- Analytics
- citation-management
- Local Marketing
- social-publishing
- MCP
- agent-native
---
