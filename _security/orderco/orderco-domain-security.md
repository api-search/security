---
api_specs:
- filename: orderco-components-api-openapi.yml
  format: yaml
  label: Order.co Components API
  slug: orderco-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-components-api-openapi.yml
- filename: orderco-incidents-api-openapi.yml
  format: yaml
  label: Order.co Incidents API
  slug: orderco-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-incidents-api-openapi.yml
- filename: orderco-maintenance-api-openapi.yml
  format: yaml
  label: Order.co Maintenance API
  slug: orderco-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-maintenance-api-openapi.yml
- filename: orderco-status-api-openapi.yml
  format: yaml
  label: Order.co Status API
  slug: orderco-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: order.co
  spf: true
hosts:
- cert_expires: Sep 29 04:42:33 2026 GMT
  host: www.order.co
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 18:22:06 2026 GMT
  host: status.order.co
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Orderco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Order.co, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Order.co
provider_slug: orderco
slug: orderco-domain-security
source_filename: orderco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.order.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:42:33 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: status.order.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 18:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: order.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/security/orderco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- Spend Management
- Accounts Payable
- Purchasing
- Vendor Management
- Payments
- Virtual Cards
- Finance Automation
- United States
---
