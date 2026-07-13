---
api_specs:
- filename: wisk-ai-openapi.yml
  format: yaml
  label: WISK Inventory & Items API
  slug: wisk-ai-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/openapi/wisk-ai-openapi.yml
- filename: wisk-ai-openapi.yml
  format: yaml
  label: WISK Venues API
  slug: wisk-ai-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/openapi/wisk-ai-openapi.yml
- filename: wisk-ai-openapi.yml
  format: yaml
  label: WISK Invoices API
  slug: wisk-ai-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/openapi/wisk-ai-openapi.yml
- filename: wisk-ai-openapi.yml
  format: yaml
  label: WISK POS Integration (Public Sales Upload) API
  slug: wisk-ai-pos-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/openapi/wisk-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wisk.ai
  spf: true
hosts:
- cert_expires: Aug 17 13:46:01 2026 GMT
  host: www.wisk.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisk Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WISK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WISK
provider_slug: wisk-ai
slug: wisk-ai-domain-security
source_filename: wisk-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wisk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 13:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wisk.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisk-ai/refs/heads/main/security/wisk-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Inventory
- Restaurant
- Bar
- Hospitality
- Cost Management
- POS Integration
---
