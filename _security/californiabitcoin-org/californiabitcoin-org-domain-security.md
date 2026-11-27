---
api_specs:
- filename: californiabitcoin-org-a2a-api-openapi.yml
  format: yaml
  label: California Bitcoin A2a API
  slug: californiabitcoin-org-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiabitcoin-org/openapi/californiabitcoin-org-a2a-api-openapi.yml
- filename: californiabitcoin-org-agent-api-openapi.yml
  format: yaml
  label: California Bitcoin Agent API
  slug: californiabitcoin-org-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiabitcoin-org/openapi/californiabitcoin-org-agent-api-openapi.yml
- filename: californiabitcoin-org-mcp-api-openapi.yml
  format: yaml
  label: California Bitcoin MCP API
  slug: californiabitcoin-org-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/californiabitcoin-org/openapi/californiabitcoin-org-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: californiabitcoin.org
  spf: false
hosts:
- cert_expires: Dec  7 11:48:33 2026 GMT
  host: californiabitcoin.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: California Bitcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Bitcoin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: California Bitcoin
provider_slug: californiabitcoin-org
slug: californiabitcoin-org-domain-security
source_filename: californiabitcoin-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: californiabitcoin.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 11:48:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: californiabitcoin.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/californiabitcoin-org/security/californiabitcoin-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin
- Education
- Cryptocurrency
- Learning
- Community
---
