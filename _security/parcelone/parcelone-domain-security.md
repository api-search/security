---
api_specs:
- filename: parcelone-closing-api-openapi.yml
  format: yaml
  label: ParcelOne Closing API
  slug: parcelone-closing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-closing-api-openapi.yml
- filename: parcelone-customer-api-openapi.yml
  format: yaml
  label: ParcelOne Customer API
  slug: parcelone-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customer-api-openapi.yml
- filename: parcelone-customs-api-openapi.yml
  format: yaml
  label: ParcelOne Customs API
  slug: parcelone-customs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-customs-api-openapi.yml
- filename: parcelone-datetime-api-openapi.yml
  format: yaml
  label: ParcelOne Datetime API
  slug: parcelone-datetime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-datetime-api-openapi.yml
- filename: parcelone-mandator-api-openapi.yml
  format: yaml
  label: ParcelOne Mandator API
  slug: parcelone-mandator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mandator-api-openapi.yml
- filename: parcelone-mobilereturn-api-openapi.yml
  format: yaml
  label: ParcelOne Mobilereturn API
  slug: parcelone-mobilereturn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-mobilereturn-api-openapi.yml
- filename: parcelone-profile-api-openapi.yml
  format: yaml
  label: ParcelOne Profile API
  slug: parcelone-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-profile-api-openapi.yml
- filename: parcelone-shipment-api-openapi.yml
  format: yaml
  label: ParcelOne Shipment API
  slug: parcelone-shipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcelone/openapi/parcelone-shipment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: parcel.one
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: parcel.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parcelone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParcelOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ParcelOne
provider_slug: parcelone
slug: parcelone-domain-security
source_filename: parcelone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcel.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parcel.one\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/parcelone/security/parcelone-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Logistics
- Shipping
- E-commerce
- Fulfillment
- International
---
