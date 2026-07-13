---
api_specs:
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Quotations API
  slug: skydropx-quotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Shipments API
  slug: skydropx-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Orders and Labels API
  slug: skydropx-orders-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Pickups API
  slug: skydropx-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Address Templates API
  slug: skydropx-address-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Tracking API
  slug: skydropx-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Finance API
  slug: skydropx-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
- filename: skydropx-openapi.yml
  format: yaml
  label: Skydropx Catalog API
  slug: skydropx-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/openapi/skydropx-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issuewild "starfieldtech.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skydropx.com
  spf: true
hosts:
- cert_expires: Sep 19 07:18:05 2026 GMT
  host: skydropx.com
  hsts: false
  http_status: 301
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 19:01:09 2026 GMT
  host: pro.skydropx.com
  hsts: false
  http_status: 302
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:38:33 2026 GMT
  host: api.skydropx.com
  hsts: false
  http_status: 302
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skydropx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skydropx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skydropx
provider_slug: skydropx
slug: skydropx-domain-security
source_filename: skydropx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:18:05 2026 GMT\n  hsts: false\n  http_status: 301\n- host: pro.skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:01:09 2026 GMT\n  hsts: false\n  http_status: 302\n- host: api.skydropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:38:33 2026 GMT\n  hsts: false\n  http_status: 302\ndomains:\n- domain: skydropx.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  All three probed hosts (skydropx.com, pro.skydropx.com, api.skydropx.com)\n  serve HTTPS over TLS 1.3 with valid certificates, but none returned an HSTS\n  (Strict-Transport-Security) response header at the time of probing. The apex\n  domain publishes a broad CAA policy and an SPF record, and a DMARC record with\n  a monitor-only policy (p=none). DNSSEC is not enabled.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydropx/refs/heads/main/security/skydropx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shipping
- Logistics
- Multi-Carrier
- Mexico
- Latin America
- Labels
- Rates
- Parcels
- Tracking
- Fulfillment
- SaaS
---
