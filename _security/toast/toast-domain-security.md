---
api_specs:
- filename: toast-orders-openapi.yaml
  format: yaml
  label: Toast Orders API
  slug: toast-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-openapi.yaml
- filename: toast-menus-openapi.yaml
  format: yaml
  label: Toast Menus API
  slug: toast-menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-openapi.yaml
- filename: toast-labor-openapi.yaml
  format: yaml
  label: Toast Labor API
  slug: toast-labor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-labor-openapi.yaml
- filename: toast-restaurants-openapi.yaml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-openapi.yaml
- filename: toast-stock-openapi.yaml
  format: yaml
  label: Toast Stock API
  slug: toast-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-openapi.yaml
- filename: toast-partners-openapi.yaml
  format: yaml
  label: Toast Partners API
  slug: toast-partners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-partners-openapi.yaml
- filename: toast-authentication-openapi.yaml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: toasttab.com
  spf: true
hosts:
- cert_expires: Sep 25 19:10:05 2026 GMT
  host: pos.toasttab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: doc.toasttab.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toast
provider_slug: toast
slug: toast-domain-security
source_filename: toast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pos.toasttab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:10:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.toasttab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: toasttab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/security/toast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Service
- Point of Sale
- Restaurants
- Hospitality
---
