---
api_specs:
- filename: toast-tab-authentication-openapi.yml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-authentication-openapi.yml
- filename: toast-tab-restaurants-openapi.yml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-restaurants-openapi.yml
- filename: toast-tab-menus-openapi.yml
  format: yaml
  label: Toast Menus API (V2)
  slug: toast-menus-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-menus-openapi.yml
- filename: toast-tab-orders-openapi.yml
  format: yaml
  label: Toast Orders API
  slug: toast-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-orders-openapi.yml
- filename: toast-tab-labor-openapi.yml
  format: yaml
  label: Toast Labor API
  slug: toast-labor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-labor-openapi.yml
- filename: toast-tab-stock-openapi.yml
  format: yaml
  label: Toast Stock API
  slug: toast-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-stock-openapi.yml
- filename: toast-tab-partners-openapi.yml
  format: yaml
  label: Toast Partners API
  slug: toast-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-partners-openapi.yml
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
- cert_expires: Sep 25 18:39:09 2026 GMT
  host: ws-api.toasttab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toast Tab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Toast
provider_slug: toast-tab
slug: toast-tab-domain-security
source_filename: toast-tab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pos.toasttab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:10:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.toasttab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: ws-api.toasttab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:39:09 2026 GMT\n  hsts: null\ndomains:\n- domain: toasttab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/security/toast-tab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Point Of Sale
- Payments
- Online Ordering
- Delivery
- Loyalty
- Gift Cards
- Menus
- Orders
- Kitchen
- Labor
- Scheduling
- Inventory
- Hospitality
- Partner Integrations
---
