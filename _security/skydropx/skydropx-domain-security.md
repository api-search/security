---
api_specs:
- filename: skydropx-address-templates-api-openapi.yml
  format: yaml
  label: Skydropx Address Templates API
  slug: skydropx-address-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-address-templates-api-openapi.yml
- filename: skydropx-authentication-api-openapi.yml
  format: yaml
  label: Skydropx Authentication API
  slug: skydropx-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-authentication-api-openapi.yml
- filename: skydropx-catalog-api-openapi.yml
  format: yaml
  label: Skydropx Catalog API
  slug: skydropx-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-catalog-api-openapi.yml
- filename: skydropx-finance-api-openapi.yml
  format: yaml
  label: Skydropx Finance API
  slug: skydropx-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-finance-api-openapi.yml
- filename: skydropx-orders-and-labels-api-openapi.yml
  format: yaml
  label: Skydropx Orders and Labels API
  slug: skydropx-orders-and-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-orders-and-labels-api-openapi.yml
- filename: skydropx-pickups-api-openapi.yml
  format: yaml
  label: Skydropx Pickups API
  slug: skydropx-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-pickups-api-openapi.yml
- filename: skydropx-quotations-api-openapi.yml
  format: yaml
  label: Skydropx Quotations API
  slug: skydropx-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-quotations-api-openapi.yml
- filename: skydropx-shipments-api-openapi.yml
  format: yaml
  label: Skydropx Shipments API
  slug: skydropx-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-shipments-api-openapi.yml
- filename: skydropx-tracking-api-openapi.yml
  format: yaml
  label: Skydropx Tracking API
  slug: skydropx-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-tracking-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "starfieldtech.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skydropx.com
  spf: true
hosts:
- cert_expires: Nov 13 09:28:43 2026 GMT
  host: www.skydropx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 19:13:10 2026 GMT
  host: pro.skydropx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 20:47:53 2026 GMT
  host: sb-pro.skydropx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Skydropx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skydropx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skydropx
provider_slug: skydropx
slug: skydropx-domain-security
source_filename: skydropx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 09:28:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pro.skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 19:13:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sb-pro.skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 20:47:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skydropx.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/security/skydropx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Multi-Carrier
- Mexico
- Latin America
- Labels
- Rates
- Parcel
- Tracking
- Fulfillment
- Software-as-a-Service
---
