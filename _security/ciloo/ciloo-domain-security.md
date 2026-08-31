---
api_specs:
- filename: ciloo-cart-api-openapi.yml
  format: yaml
  label: Ciloo Cart API
  slug: ciloo-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/openapi/ciloo-cart-api-openapi.yml
- filename: ciloo-authentication-api-openapi.yml
  format: yaml
  label: Ciloo Authentication API
  slug: ciloo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/openapi/ciloo-authentication-api-openapi.yml
- filename: ciloo-customers-api-openapi.yml
  format: yaml
  label: Ciloo Customers API
  slug: ciloo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/openapi/ciloo-customers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ciloo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cilooprint.com
  spf: true
hosts:
- cert_expires: Oct 18 12:03:44 2026 GMT
  host: ciloo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:29:43 2026 GMT
  host: api.cilooprint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:44:57 2026 GMT
  host: dashboard.cilooprint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ciloo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ciloo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ciloo
provider_slug: ciloo
slug: ciloo-domain-security
source_filename: ciloo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ciloo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:03:44 2026 GMT\n  hsts: false\n- host: api.cilooprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:29:43 2026 GMT\n  hsts: false\n- host: dashboard.cilooprint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ciloo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cilooprint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciloo/refs/heads/main/security/ciloo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Printing
- Branded Merchandise
- Promotional Products
- Print On Demand
- E-Commerce
- Digital Asset Management
- Procurement
- Fulfillment
- Marketing
---
