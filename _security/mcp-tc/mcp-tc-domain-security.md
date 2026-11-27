---
api_specs:
- filename: mcp-tc-directory-api-openapi.yml
  format: yaml
  label: MCP Directory API
  slug: mcp-tc-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-tc/openapi/mcp-tc-directory-api-openapi.yml
- filename: mcp-tc-registry-api-openapi.yml
  format: yaml
  label: MCP Registry API
  slug: mcp-tc-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-tc/openapi/mcp-tc-registry-api-openapi.yml
- filename: mcp-tc-submit-api-openapi.yml
  format: yaml
  label: MCP Submit API
  slug: mcp-tc-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-tc/openapi/mcp-tc-submit-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mcp.tc
  spf: true
hosts:
- cert_expires: Jan  1 09:15:03 2027 GMT
  host: mcp.tc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MCP
provider_slug: mcp-tc
slug: mcp-tc-domain-security
source_filename: mcp-tc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp.tc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 09:15:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcp.tc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcp-tc/security/mcp-tc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Directory
- Artificial Intelligence
- Tools
- Open Source
- Community
---
