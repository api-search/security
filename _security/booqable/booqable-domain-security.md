---
api_specs:
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Orders API
  slug: booqable-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Order Fulfillment API
  slug: booqable-order-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Products API
  slug: booqable-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Product Groups API
  slug: booqable-product-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Customers API
  slug: booqable-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Stock Items API
  slug: booqable-stock-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Availability API
  slug: booqable-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Documents & Invoices API
  slug: booqable-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Bundles & Collections API
  slug: booqable-bundles-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Webhooks API
  slug: booqable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
- filename: booqable-openapi.yml
  format: yaml
  label: Booqable Settings & Locations API
  slug: booqable-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/openapi/booqable-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: booqable.com
  spf: true
hosts:
- cert_expires: Sep 28 15:05:18 2026 GMT
  host: booqable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 07:26:58 2026 GMT
  host: developers.booqable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Booqable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booqable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Booqable
provider_slug: booqable
slug: booqable-domain-security
source_filename: booqable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: booqable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.booqable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:26:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: booqable.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booqable/refs/heads/main/security/booqable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Rental Management
- Inventory
- Equipment Rental
- Bookings
- Orders
- E-commerce
- JSON:API
---
