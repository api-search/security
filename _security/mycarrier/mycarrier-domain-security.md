---
api_specs:
- filename: mycarrier-public-api-openapi.json
  format: json
  label: MyCarrier Public API
  slug: mycarrier-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-public-api-openapi.json
- filename: mycarrier-order-public-api-openapi.json
  format: json
  label: MyCarrier Order API
  slug: mycarrier-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-order-public-api-openapi.json
- filename: mycarrier-freightaudit-api-openapi.json
  format: json
  label: MyCarrier FreightAudit API
  slug: mycarrier-freightaudit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-freightaudit-api-openapi.json
- filename: mycarrier-webhook-api-openapi.json
  format: json
  label: MyCarrier Webhook Registration API
  slug: mycarrier-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-webhook-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mycarrier.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mycarriertms.com
  spf: true
hosts:
- cert_expires: Oct 17 20:19:27 2026 GMT
  host: go.mycarrier.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 10:15:22 2026 GMT
  host: developer.mycarrier.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:47:44 2026 GMT
  host: api.mycarriertms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mycarrier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyCarrier, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MyCarrier
provider_slug: mycarrier
slug: mycarrier-domain-security
source_filename: mycarrier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go.mycarrier.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 20:19:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.mycarrier.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:15:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mycarriertms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:47:44 2026 GMT\n  hsts: null\ndomains:\n- domain: mycarrier.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mycarriertms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/security/mycarrier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Transportation
- Freight
- Shipping
- LTL
- Supply Chain
- Transportation Management
- Freight Audit
- Invoicing
---
