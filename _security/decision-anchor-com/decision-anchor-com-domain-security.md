---
api_specs:
- filename: decision-anchor-com-openapi.yml
  format: yaml
  label: Decision Anchor API
  slug: decision-anchor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decision-anchor-com/refs/heads/main/openapi/decision-anchor-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: decision-anchor.com
  spf: true
hosts:
- cert_expires: Nov  7 10:11:36 2026 GMT
  host: decision-anchor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 21:16:48 2026 GMT
  host: api.decision-anchor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 21:16:48 2026 GMT
  host: mcp.decision-anchor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Decision Anchor Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decision Anchor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Decision Anchor
provider_slug: decision-anchor-com
slug: decision-anchor-com-domain-security
source_filename: decision-anchor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decision-anchor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 10:11:36 2026 GMT\n  hsts: false\n- host: api.decision-anchor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 21:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.decision-anchor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 21:16:48 2026 GMT\n  hsts: false\ndomains:\n- domain: decision-anchor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decision-anchor-com/refs/heads/main/security/decision-anchor-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agent Accountability
- Decision Records
- Audit Trail
- A2A
- MCP
- x402
- Agentic Commerce
- Multi-Agent Systems
- Agent-Native
- South Korea
---
