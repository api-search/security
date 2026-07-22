---
api_specs:
- filename: zaius-events-openapi.json
  format: json
  label: ODP Events API
  slug: odp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-events-openapi.json
- filename: zaius-customers-openapi.json
  format: json
  label: ODP Customers API
  slug: odp-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-customers-openapi.json
- filename: zaius-orders-openapi.json
  format: json
  label: ODP Orders API
  slug: odp-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-orders-openapi.json
- filename: zaius-products-openapi.json
  format: json
  label: ODP Products API
  slug: odp-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-products-openapi.json
- filename: zaius-objects-openapi.json
  format: json
  label: ODP Objects API
  slug: odp-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-objects-openapi.json
- filename: zaius-lists-openapi.json
  format: json
  label: ODP Lists API
  slug: odp-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-lists-openapi.json
- filename: zaius-consent-openapi.json
  format: json
  label: ODP Consent API
  slug: odp-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-consent-openapi.json
- filename: zaius-exports-openapi.json
  format: json
  label: ODP Exports API
  slug: odp-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-exports-openapi.json
- filename: zaius-recommendations-openapi.json
  format: json
  label: ODP Recommendations API
  slug: odp-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-recommendations-openapi.json
- filename: zaius-realtimesegments-openapi.json
  format: json
  label: ODP Real-Time Segments API
  slug: odp-real-time-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-realtimesegments-openapi.json
- filename: zaius-advanced-openapi.json
  format: json
  label: ODP Advanced API (schema, identifiers, compliance)
  slug: odp-advanced-api-schema-identifiers-compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/openapi/zaius-advanced-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zaius.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optimizely.com
  spf: true
hosts:
- cert_expires: Sep  3 22:33:20 2026 GMT
  host: www.zaius.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.us1.odp.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: api.eu1.odp.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zaius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zaius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zaius
provider_slug: zaius
slug: zaius-domain-security
source_filename: zaius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zaius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 22:33:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us1.odp.optimizely.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu1.odp.optimizely.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zaius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: optimizely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zaius/refs/heads/main/security/zaius-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Data Platform
- CDP
- Marketing
- Personalization
- Segmentation
- Ecommerce
- Customer Data
- Real-Time Audiences
- Events
---
