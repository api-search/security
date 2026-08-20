---
api_specs:
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API
  slug: happyrobot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
- filename: happyrobot-platform-v1-openapi.json
  format: json
  label: Happyrobot Platform API v1
  slug: happyrobot-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-platform-v1-openapi.json
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API (EU cluster)
  slug: happyrobot-public-api-eu-cluster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: happyrobot.ai
  spf: true
hosts:
- cert_expires: Sep  7 21:04:26 2026 GMT
  host: www.happyrobot.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:05:11 2026 GMT
  host: docs.happyrobot.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:09:38 2026 GMT
  host: platform.happyrobot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happyrobot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Happyrobot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Happyrobot
provider_slug: happyrobot
slug: happyrobot-domain-security
source_filename: happyrobot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.happyrobot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:04:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.happyrobot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.happyrobot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:09:38 2026 GMT\n  hsts: null\ndomains:\n- domain: happyrobot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/security/happyrobot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Agent Orchestration
- Voice AI
- Conversational AI
- Logistics
- Freight
- Supply Chain
- Workflow-Automation
- Contact Center
- Telephony
- MCP
- agent-native
- Agent Governance
- Enterprise Automation
---
