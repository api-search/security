---
api_specs:
- filename: agentmail-openapi-original.yml
  format: yaml
  label: AgentMail API
  slug: agentmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentmail/refs/heads/main/openapi/agentmail-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentmail.to
  spf: false
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.agentmail.to
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: x402.api.agentmail.to
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: mpp.api.agentmail.to
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentmail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentMail, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: AgentMail
provider_slug: agentmail
slug: agentmail-domain-security
source_filename: agentmail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.agentmail.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\n- host: x402.api.agentmail.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\n- host: mpp.api.agentmail.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agentmail.to\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentmail/refs/heads/main/security/agentmail-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Email
- API
- AI Agents
- Inbox
- Messaging
- Webhooks
- WebSockets
- SMTP
- IMAP
- MCP
- Agentic
- Developer Tools
---
