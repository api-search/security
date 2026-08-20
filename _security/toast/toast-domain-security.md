---
api_specs:
- filename: toast-authentication-api-openapi.yml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-api-openapi.yml
- filename: toast-connectedrestaurants-api-openapi.yml
  format: yaml
  label: Toast ConnectedRestaurants API
  slug: toast-connectedrestaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-connectedrestaurants-api-openapi.yml
- filename: toast-discounts-api-openapi.yml
  format: yaml
  label: Toast Discounts API
  slug: toast-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-discounts-api-openapi.yml
- filename: toast-employees-api-openapi.yml
  format: yaml
  label: Toast Employees API
  slug: toast-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-employees-api-openapi.yml
- filename: toast-groups-api-openapi.yml
  format: yaml
  label: Toast Groups API
  slug: toast-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-groups-api-openapi.yml
- filename: toast-jobs-api-openapi.yml
  format: yaml
  label: Toast Jobs API
  slug: toast-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-jobs-api-openapi.yml
- filename: toast-menus-api-openapi.yml
  format: yaml
  label: Toast Menus API
  slug: toast-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-api-openapi.yml
- filename: toast-metadata-api-openapi.yml
  format: yaml
  label: Toast Metadata API
  slug: toast-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-metadata-api-openapi.yml
- filename: toast-orders-api-openapi.yml
  format: yaml
  label: Toast Orders API
  slug: toast-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-api-openapi.yml
- filename: toast-payments-api-openapi.yml
  format: yaml
  label: Toast Payments API
  slug: toast-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-payments-api-openapi.yml
- filename: toast-restaurants-api-openapi.yml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-api-openapi.yml
- filename: toast-shifts-api-openapi.yml
  format: yaml
  label: Toast Shifts API
  slug: toast-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-shifts-api-openapi.yml
- filename: toast-stock-api-openapi.yml
  format: yaml
  label: Toast Stock API
  slug: toast-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-api-openapi.yml
- filename: toast-time-entries-api-openapi.yml
  format: yaml
  label: Toast Time entries API
  slug: toast-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-time-entries-api-openapi.yml
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
- Point-of-Sale
- Restaurant
- Hospitality
---
