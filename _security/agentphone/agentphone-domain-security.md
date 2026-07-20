---
api_specs:
- filename: agentphone-openapi-original.json
  format: json
  label: AgentPhone API
  slug: agentphone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/openapi/agentphone-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentphone.ai
  spf: true
hosts:
- cert_expires: Oct  1 10:23:20 2026 GMT
  host: api.agentphone.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentPhone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgentPhone
provider_slug: agentphone
slug: agentphone-domain-security
source_filename: agentphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.agentphone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:23:20 2026 GMT\n  hsts: null\ndomains:\n- domain: agentphone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentphone/refs/heads/main/security/agentphone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telephony
- Phone Numbers
- SMS
- Voice
- AI Agents
- Messaging
- Communications
- Webhooks
- MCP
- iMessage
---
