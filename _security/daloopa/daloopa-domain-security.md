---
api_specs:
- filename: daloopa-api-openapi.yml
  format: yaml
  label: Daloopa API v3
  slug: daloopa-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-api-openapi.yml
- filename: daloopa-mcp-service-openapi.json
  format: json
  label: Daloopa MCP Server
  slug: daloopa-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/openapi/daloopa-mcp-service-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: daloopa.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: daloopa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 04:54:09 2026 GMT
  host: docs.daloopa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: app.daloopa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daloopa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daloopa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Daloopa
provider_slug: daloopa
slug: daloopa-domain-security
source_filename: daloopa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daloopa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.daloopa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 04:54:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.daloopa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: daloopa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daloopa/refs/heads/main/security/daloopa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- financial-data
- fundamental-data
- market-data
- investment-research
- equity-research
- sec-filings
- earnings
- fintech
- mcp
- agent-native
- agent-skills
- webhooks
- data-warehouse
---
