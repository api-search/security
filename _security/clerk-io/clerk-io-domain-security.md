---
api_specs:
- filename: clerk-io-accessories-api-openapi.yml
  format: yaml
  label: Clerk.io Accessories API
  slug: clerk-io-accessories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-accessories-api-openapi.yml
- filename: clerk-io-audiences-api-openapi.yml
  format: yaml
  label: Clerk.io Audiences API
  slug: clerk-io-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-audiences-api-openapi.yml
- filename: clerk-io-campaigns-api-openapi.yml
  format: yaml
  label: Clerk.io Campaigns API
  slug: clerk-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-campaigns-api-openapi.yml
- filename: clerk-io-catalog-api-openapi.yml
  format: yaml
  label: Clerk.io Catalog API
  slug: clerk-io-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-catalog-api-openapi.yml
- filename: clerk-io-logging-api-openapi.yml
  format: yaml
  label: Clerk.io Logging API
  slug: clerk-io-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-logging-api-openapi.yml
- filename: clerk-io-merchandising-api-openapi.yml
  format: yaml
  label: Clerk.io Merchandising API
  slug: clerk-io-merchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-merchandising-api-openapi.yml
- filename: clerk-io-parcels-api-openapi.yml
  format: yaml
  label: Clerk.io Parcels API
  slug: clerk-io-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-parcels-api-openapi.yml
- filename: clerk-io-privacy-api-openapi.yml
  format: yaml
  label: Clerk.io Privacy API
  slug: clerk-io-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-privacy-api-openapi.yml
- filename: clerk-io-product-data-api-openapi.yml
  format: yaml
  label: Clerk.io Product Data API
  slug: clerk-io-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-product-data-api-openapi.yml
- filename: clerk-io-recommendations-api-openapi.yml
  format: yaml
  label: Clerk.io Recommendations API
  slug: clerk-io-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-recommendations-api-openapi.yml
- filename: clerk-io-search-api-openapi.yml
  format: yaml
  label: Clerk.io Search API
  slug: clerk-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-search-api-openapi.yml
- filename: clerk-io-subscribers-api-openapi.yml
  format: yaml
  label: Clerk.io Subscribers API
  slug: clerk-io-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-subscribers-api-openapi.yml
- filename: clerk-io-tokens-api-openapi.yml
  format: yaml
  label: Clerk.io Tokens API
  slug: clerk-io-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-tokens-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:product-devops@clerk.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clerk.io
  spf: true
hosts:
- cert_expires: Nov 10 14:31:44 2026 GMT
  host: www.clerk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:42:59 2026 GMT
  host: docs.clerk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.clerk.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clerk Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerk.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clerk.io
provider_slug: clerk-io
slug: clerk-io-domain-security
source_filename: clerk-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clerk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:31:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clerk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clerk.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clerk.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:product-devops@clerk.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/security/clerk-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Commerce
- E-Commerce
- Email Marketing
- Personalization
- Recommendations
- Search
---
