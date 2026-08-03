---
api_specs:
- filename: lucid-rest-api-openapi.yml
  format: yaml
  label: Lucid REST API
  slug: lucid-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-rest-api-openapi.yml
- filename: lucid-data-api-openapi.yml
  format: yaml
  label: Lucid Data API
  slug: lucid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-data-api-openapi.yml
- filename: lucid-scim-api-openapi.yml
  format: yaml
  label: Lucid SCIM API
  slug: lucid-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-scim-api-openapi.yml
- filename: lucid-chatgpt-plugin-openapi.yaml
  format: yaml
  label: Lucid ChatGPT Plugin API
  slug: lucid-chatgpt-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-chatgpt-plugin-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucid.co
  spf: true
hosts:
- cert_expires: Oct 12 04:24:07 2026 GMT
  host: lucid.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 03:57:52 2026 GMT
  host: developer.lucid.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 22:59:28 2026 GMT
  host: api.lucid.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucid
provider_slug: lucid
slug: lucid-domain-security
source_filename: lucid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:24:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lucid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:57:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lucid.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:59:28 2026 GMT\n  hsts: null\ndomains:\n- domain: lucid.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/security/lucid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Visual Collaboration
- Diagramming
- Whiteboarding
- Productivity
- SaaS
- Cloud Visualization
- SCIM
- Identity
- Data
- MCP
---
