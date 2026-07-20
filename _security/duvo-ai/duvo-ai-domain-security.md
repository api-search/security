---
api_specs:
- filename: duvo-ai-openapi-original.json
  format: json
  label: Duvo Public API
  slug: duvo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/openapi/duvo-ai-openapi-original.json
description: ''
domains:
- caa:
  - sites.framer.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: duvo.ai
  spf: true
hosts:
- cert_expires: Aug 16 00:55:41 2026 GMT
  host: www.duvo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:46:38 2026 GMT
  host: api.duvo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duvo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duvo Ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Duvo Ai
provider_slug: duvo-ai
slug: duvo-ai-domain-security
source_filename: duvo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duvo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:55:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.duvo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:46:38 2026 GMT\n  hsts: null\ndomains:\n- domain: duvo.ai\n  dnssec: true\n  caa:\n  - sites.framer.app.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duvo-ai/refs/heads/main/security/duvo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise; Ai
- Process Intelligence
- Automation
- Agents
- SAP Migration
- Operations
- ERP
- Transformation
- Approvals
- Audit
- MCP
---
