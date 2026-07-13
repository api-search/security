---
api_specs:
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Shipments API
  slug: parcelperform-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Tracking Events API
  slug: parcelperform-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Returns API
  slug: parcelperform-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Webhooks API
  slug: parcelperform-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Couriers API
  slug: parcelperform-couriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Analytics API
  slug: parcelperform-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parcelperform.com
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.parcelperform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:05:09 2026 GMT
  host: developers.parcelperform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.parcelperform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parcelperform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parcel Perform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parcel Perform
provider_slug: parcelperform
slug: parcelperform-domain-security
source_filename: parcelperform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parcelperform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.parcelperform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:05:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.parcelperform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: parcelperform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/security/parcelperform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Shipment Tracking
- Post-Purchase
- Delivery Experience
- Returns
- E-Commerce
---
