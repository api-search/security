---
api_specs:
- filename: textql-v2-openapi.yml
  format: yaml
  label: TextQL v2 API
  slug: textql-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-v2-openapi.yml
- filename: textql-chat-v1-openapi.yml
  format: yaml
  label: TextQL Platform API (v1)
  slug: textql-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-chat-v1-openapi.yml
- filename: textql-platform-api-openapi.yml
  format: yaml
  label: TextQL Public RPC API
  slug: textql-public-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/openapi/textql-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: textql.com
  spf: true
hosts:
- cert_expires: Oct 21 01:44:22 2026 GMT
  host: textql.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 11:38:37 2026 GMT
  host: docs.textql.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 11:38:37 2026 GMT
  host: app.textql.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TextQL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TextQL
provider_slug: textql
slug: textql-domain-security
source_filename: textql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 01:44:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.textql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: app.textql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: textql.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textql/refs/heads/main/security/textql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Analytics
- Business Intelligence
- Data
- Agents
- MCP
- Semantic Layer
- Text-to-SQL
- Data Warehouse
- Enterprise
---
