---
api_specs:
- filename: dexio-dexio-api-api-openapi.yml
  format: yaml
  label: Dexio Dexio API
  slug: dexio-dexio-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/openapi/dexio-dexio-api-api-openapi.yml
- filename: dexio-install-api-openapi.yml
  format: yaml
  label: Dexio Install API
  slug: dexio-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/openapi/dexio-install-api-openapi.yml
- filename: dexio-mcp-api-openapi.yml
  format: yaml
  label: Dexio MCP API
  slug: dexio-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/openapi/dexio-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dexio.wiki
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: dexio.wiki
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dexio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dexio
provider_slug: dexio
slug: dexio-domain-security
source_filename: dexio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexio.wiki\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dexio.wiki\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexio/refs/heads/main/security/dexio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Wiki
- Knowledge Management
- Agent-Integration
- Open Source
---
