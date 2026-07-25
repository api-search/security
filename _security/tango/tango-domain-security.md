---
api_specs:
- filename: tango-accounts-api-openapi.yml
  format: yaml
  label: Tango Accounts API
  slug: tango-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-accounts-api-openapi.yml
- filename: tango-catalog-api-openapi.yml
  format: yaml
  label: Tango Catalog API
  slug: tango-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-catalog-api-openapi.yml
- filename: tango-customers-api-openapi.yml
  format: yaml
  label: Tango Customers API
  slug: tango-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-customers-api-openapi.yml
- filename: tango-digital-templates-api-openapi.yml
  format: yaml
  label: Tango Digital Templates API
  slug: tango-digital-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-digital-templates-api-openapi.yml
- filename: tango-funding-api-openapi.yml
  format: yaml
  label: Tango Funding API
  slug: tango-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-funding-api-openapi.yml
- filename: tango-line-items-api-openapi.yml
  format: yaml
  label: Tango Line Items API
  slug: tango-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-line-items-api-openapi.yml
- filename: tango-low-balance-alerts-api-openapi.yml
  format: yaml
  label: Tango Low Balance Alerts API
  slug: tango-low-balance-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-low-balance-alerts-api-openapi.yml
- filename: tango-orders-api-openapi.yml
  format: yaml
  label: Tango Orders API
  slug: tango-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-orders-api-openapi.yml
- filename: tango-reference-data-api-openapi.yml
  format: yaml
  label: Tango Reference Data API
  slug: tango-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/openapi/tango-reference-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tangocard.com
  spf: true
hosts:
- cert_expires: Aug 24 15:43:14 2026 GMT
  host: www.tangocard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:11:01 2026 GMT
  host: developers.tangocard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.tangocard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tango, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tango
provider_slug: tango
slug: tango-domain-security
source_filename: tango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tangocard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:43:14 2026 GMT\n  hsts: false\n- host: developers.tangocard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:11:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tangocard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tangocard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango/refs/heads/main/security/tango-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Catalog Management
- Digital Rewards
- Gift Cards
- Incentives
- Loyalty
- Rewards As A Service
---
