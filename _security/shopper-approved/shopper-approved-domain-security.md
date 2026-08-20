---
api_specs:
- filename: shopper-approved-orders-api-openapi.yml
  format: yaml
  label: Shopper Approved Orders API
  slug: shopper-approved-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/openapi/shopper-approved-orders-api-openapi.yml
- filename: shopper-approved-product-reviews-api-openapi.yml
  format: yaml
  label: Shopper Approved Product Reviews API
  slug: shopper-approved-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/openapi/shopper-approved-product-reviews-api-openapi.yml
- filename: shopper-approved-reviews-api-openapi.yml
  format: yaml
  label: Shopper Approved Reviews API
  slug: shopper-approved-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/openapi/shopper-approved-reviews-api-openapi.yml
- filename: shopper-approved-statistics-api-openapi.yml
  format: yaml
  label: Shopper Approved Statistics API
  slug: shopper-approved-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/openapi/shopper-approved-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopperapproved.com
  spf: true
hosts:
- cert_expires: Oct  8 19:50:35 2026 GMT
  host: help.shopperapproved.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:50:35 2026 GMT
  host: api.shopperapproved.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopper Approved Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopper Approved, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shopper Approved
provider_slug: shopper-approved
slug: shopper-approved-domain-security
source_filename: shopper-approved-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.shopperapproved.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:50:35 2026 GMT\n  hsts: false\n- host: api.shopperapproved.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:50:35 2026 GMT\n  hsts: null\ndomains:\n- domain: shopperapproved.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopper-approved/refs/heads/main/security/shopper-approved-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Reviews
- Ratings
- E-Commerce
- Customer Feedback
- Social Proof
---
