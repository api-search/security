---
api_specs:
- filename: amuncore-dynamic-api-openapi.yml
  format: yaml
  label: AmunCore API
  slug: amuncore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/openapi/amuncore-dynamic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amuncore.com
  spf: true
hosts:
- cert_expires: Aug 26 21:36:44 2026 GMT
  host: amuncore.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amuncore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmunCore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AmunCore
provider_slug: amuncore
slug: amuncore-domain-security
source_filename: amuncore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amuncore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: amuncore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/security/amuncore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- API Management
- Backend
- No-Code
- SQL
- PostgreSQL
- MySQL
- Oracle
- MCP
- Agents
- Data
- SQL Server
- Webhook
- OpenAPI
- Low-Code
- Egypt
---
