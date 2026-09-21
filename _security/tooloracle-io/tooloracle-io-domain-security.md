---
api_specs:
- filename: tooloracle-io-mcp-platform-openapi.yml
  format: yaml
  label: ToolOracle MCP Platform API
  slug: tooloracle-mcp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-mcp-platform-openapi.yml
- filename: tooloracle-io-x402-v2-openapi.yml
  format: yaml
  label: ToolOracle x402 v2 Compliance, Evidence & Agent-Safety API
  slug: tooloracle-x402-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-x402-v2-openapi.yml
- filename: tooloracle-io-feedoracle-compliance-evidence-openapi.yml
  format: yaml
  label: FeedOracle Compliance Evidence API
  slug: feedoracle-compliance-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/openapi/tooloracle-io-feedoracle-compliance-evidence-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tooloracle.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feedoracle.io
  spf: true
hosts:
- cert_expires: Dec 12 20:45:50 2026 GMT
  host: tooloracle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 19:14:34 2026 GMT
  host: feedoracle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 02:54:49 2026 GMT
  host: api.feedoracle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Tooloracle Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FeedOracle Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FeedOracle Technologies
provider_slug: tooloracle-io
slug: tooloracle-io-domain-security
source_filename: tooloracle-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tooloracle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 20:45:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: feedoracle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:14:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.feedoracle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tooloracle.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: feedoracle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooloracle-io/refs/heads/main/security/tooloracle-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- MCP
- Agent Infrastructure
- A2A
- x402
- Micropayments
- Compliance
- RegTech
- Blockchain
- Sanctions Screening
- Agent Discovery
- Germany
---
