---
api_specs:
- filename: toast-tab-authentication-api-openapi.yml
  format: yaml
  label: Toast Authentication API
  slug: toast-tab-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-authentication-api-openapi.yml
- filename: toast-tab-connectedrestaurants-api-openapi.yml
  format: yaml
  label: Toast ConnectedRestaurants API
  slug: toast-tab-connectedrestaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-connectedrestaurants-api-openapi.yml
- filename: toast-tab-discounts-api-openapi.yml
  format: yaml
  label: Toast Discounts API
  slug: toast-tab-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-discounts-api-openapi.yml
- filename: toast-tab-employees-api-openapi.yml
  format: yaml
  label: Toast Employees API
  slug: toast-tab-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-employees-api-openapi.yml
- filename: toast-tab-groups-api-openapi.yml
  format: yaml
  label: Toast Groups API
  slug: toast-tab-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-groups-api-openapi.yml
- filename: toast-tab-jobs-api-openapi.yml
  format: yaml
  label: Toast Jobs API
  slug: toast-tab-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-jobs-api-openapi.yml
- filename: toast-tab-menus-api-openapi.yml
  format: yaml
  label: Toast Menus API
  slug: toast-tab-menus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-menus-api-openapi.yml
- filename: toast-tab-metadata-api-openapi.yml
  format: yaml
  label: Toast Metadata API
  slug: toast-tab-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-metadata-api-openapi.yml
- filename: toast-tab-orders-api-openapi.yml
  format: yaml
  label: Toast Orders API
  slug: toast-tab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-orders-api-openapi.yml
- filename: toast-tab-payments-api-openapi.yml
  format: yaml
  label: Toast Payments API
  slug: toast-tab-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-payments-api-openapi.yml
- filename: toast-tab-restaurants-api-openapi.yml
  format: yaml
  label: Toast Restaurants API
  slug: toast-tab-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-restaurants-api-openapi.yml
- filename: toast-tab-shifts-api-openapi.yml
  format: yaml
  label: Toast Shifts API
  slug: toast-tab-shifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-shifts-api-openapi.yml
- filename: toast-tab-stock-api-openapi.yml
  format: yaml
  label: Toast Stock API
  slug: toast-tab-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-stock-api-openapi.yml
- filename: toast-tab-time-entries-api-openapi.yml
  format: yaml
  label: Toast Time entries API
  slug: toast-tab-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast-tab/refs/heads/main/openapi/toast-tab-time-entries-api-openapi.yml
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
