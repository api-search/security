---
api_specs:
- filename: medusa-store-openapi.yaml
  format: yaml
  label: Medusa Store API
  slug: medusa-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-store-openapi.yaml
- filename: medusa-admin-openapi.yaml
  format: yaml
  label: Medusa Admin API
  slug: medusa-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-admin-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medusajs.com
  spf: true
hosts:
- cert_expires: Oct 20 10:25:09 2026 GMT
  host: medusajs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 15:39:34 2026 GMT
  host: docs.medusajs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.medusajs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Medusa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medusa, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medusa
provider_slug: medusa
slug: medusa-domain-security
source_filename: medusa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medusajs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 10:25:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.medusajs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 15:39:34 2026 GMT\n  hsts: false\n- host: api.medusajs.com\n  https: false\ndomains:\n- domain: medusajs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/security/medusa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Headless Commerce
- Open-Source
- Commerce
- Storefront
- Order Management
- Node.js
- GraphQL
- Agentic Commerce
- MCP
---
