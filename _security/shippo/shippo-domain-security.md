---
api_specs:
- filename: shippo-addresses-api-openapi.yml
  format: yaml
  label: Shippo Addresses API
  slug: shippo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-addresses-api-openapi.yml
- filename: shippo-carrier-accounts-api-openapi.yml
  format: yaml
  label: Shippo Carrier Accounts API
  slug: shippo-carrier-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-carrier-accounts-api-openapi.yml
- filename: shippo-parcels-api-openapi.yml
  format: yaml
  label: Shippo Parcels API
  slug: shippo-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-parcels-api-openapi.yml
- filename: shippo-rates-api-openapi.yml
  format: yaml
  label: Shippo Rates API
  slug: shippo-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-rates-api-openapi.yml
- filename: shippo-refunds-api-openapi.yml
  format: yaml
  label: Shippo Refunds API
  slug: shippo-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-refunds-api-openapi.yml
- filename: shippo-shipments-api-openapi.yml
  format: yaml
  label: Shippo Shipments API
  slug: shippo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-shipments-api-openapi.yml
- filename: shippo-tracking-api-openapi.yml
  format: yaml
  label: Shippo Tracking API
  slug: shippo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-tracking-api-openapi.yml
- filename: shippo-transactions-api-openapi.yml
  format: yaml
  label: Shippo Transactions API
  slug: shippo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-transactions-api-openapi.yml
- filename: shippo-webhooks-api-openapi.yml
  format: yaml
  label: Shippo Webhooks API
  slug: shippo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goshippo.com
  spf: true
hosts:
- cert_expires: Aug 12 10:36:37 2026 GMT
  host: goshippo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:43:31 2026 GMT
  host: docs.goshippo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: api.goshippo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shippo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shippo
provider_slug: shippo
slug: shippo-domain-security
source_filename: shippo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:36:37 2026 GMT\n  hsts: false\n- host: docs.goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goshippo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/security/shippo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Labels
- Logistics
- Returns
- Shipping
- Tracking
---
