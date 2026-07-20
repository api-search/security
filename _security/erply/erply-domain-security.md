---
api_specs:
- filename: erply-pim-openapi.json
  format: json
  label: Erply PIM API
  slug: erply-pim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-pim-openapi.json
- filename: erply-assignments-openapi.json
  format: json
  label: Erply Assignments API
  slug: erply-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-assignments-openapi.json
- filename: erply-cafa-openapi.json
  format: json
  label: Erply CAFA API
  slug: erply-cafa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-cafa-openapi.json
- filename: erply-webhook-openapi.json
  format: json
  label: Erply Webhook Manager API
  slug: erply-webhook-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-webhook-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: erply.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: erply.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Erply
provider_slug: erply
slug: erply-domain-security
source_filename: erply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: erply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/security/erply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Point of Sale
- Inventory
- Product Information Management
- CRM
- Ecommerce
- Warehouse Management
- Webhooks
- Company
---
