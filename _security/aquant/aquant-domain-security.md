---
api_specs:
- filename: aquant-mcp-server-openapi.json
  format: json
  label: Aquant MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-mcp-server-openapi.json
- filename: aquant-voiceai-api-openapi.json
  format: json
  label: Aquant Conversation Platform (VoiceAI) API
  slug: acp-voiceai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-voiceai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aquant.ai
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Oct 23 16:11:44 2026 GMT
  host: www.aquant.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 21:32:12 2026 GMT
  host: mcp.aquant.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:22:28 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aquant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aquant, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aquant
provider_slug: aquant
slug: aquant-domain-security
source_filename: aquant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aquant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 16:11:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.aquant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:32:12 2026 GMT\n  hsts: null\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:22:28 2026 GMT\n  hsts: null\ndomains:\n- domain: aquant.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/security/aquant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Field Service
- Service Management
- Manufacturing
- Medical Devices
- Industrial Equipment
- Knowledge-Management
- Voice AI
- MCP
- Predictive Maintenance
---
