---
api_specs:
- filename: blue-yonder-inventory-api-openapi.yml
  format: yaml
  label: blue-yonder Inventory API
  slug: blue-yonder-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-inventory-api-openapi.yml
- filename: blue-yonder-orders-api-openapi.yml
  format: yaml
  label: blue-yonder Orders API
  slug: blue-yonder-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-orders-api-openapi.yml
- filename: blue-yonder-receipts-api-openapi.yml
  format: yaml
  label: blue-yonder Receipts API
  slug: blue-yonder-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-receipts-api-openapi.yml
- filename: blue-yonder-tasks-api-openapi.yml
  format: yaml
  label: blue-yonder Tasks API
  slug: blue-yonder-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/openapi/blue-yonder-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueyonder.com
  spf: true
hosts:
- cert_expires: Oct  9 11:35:54 2026 GMT
  host: blueyonder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 11:35:54 2026 GMT
  host: info.blueyonder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blue Yonder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for blue-yonder, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: blue-yonder
provider_slug: blue-yonder
slug: blue-yonder-domain-security
source_filename: blue-yonder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueyonder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:35:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: info.blueyonder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:35:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blueyonder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-yonder/refs/heads/main/security/blue-yonder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
