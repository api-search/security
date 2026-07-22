---
api_specs:
- filename: roadsync-rspay-openapi.json
  format: json
  label: RoadSyncPay Public API
  slug: roadsyncpay-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-rspay-openapi.json
- filename: roadsync-invoice-openapi.json
  format: json
  label: Invoice API
  slug: invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-invoice-openapi.json
- filename: roadsync-company-openapi.json
  format: json
  label: Company API
  slug: company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-company-openapi.json
- filename: roadsync-workorder-openapi.json
  format: json
  label: WorkOrders API
  slug: workorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-workorder-openapi.json
- filename: roadsync-payment-openapi.json
  format: json
  label: Payment API
  slug: payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-payment-openapi.json
- filename: roadsync-client-api-openapi.json
  format: json
  label: Legacy Client API
  slug: legacy-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/openapi/roadsync-client-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roadsync.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: roadsync.app
  spf: true
hosts:
- cert_expires: Sep 23 02:22:38 2026 GMT
  host: www.roadsync.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: test.api.roadsync.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.roadsync.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roadsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roadsync, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Roadsync
provider_slug: roadsync
slug: roadsync-domain-security
source_filename: roadsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roadsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: test.api.roadsync.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\n- host: api.roadsync.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: roadsync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: roadsync.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadsync/refs/heads/main/security/roadsync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Payments
- Logistics
- Trucking
- Invoicing
- Transportation
- Fintech
---
