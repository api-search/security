---
api_specs:
- filename: rubiconnect-campaigns-api-openapi.yml
  format: yaml
  label: RubiConnect Campaigns API
  slug: rubiconnect-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-campaigns-api-openapi.yml
- filename: rubiconnect-capabilities-api-openapi.yml
  format: yaml
  label: RubiConnect Capabilities API
  slug: rubiconnect-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-capabilities-api-openapi.yml
- filename: rubiconnect-messages-api-openapi.yml
  format: yaml
  label: RubiConnect Messages API
  slug: rubiconnect-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-messages-api-openapi.yml
- filename: rubiconnect-webhooks-api-openapi.yml
  format: yaml
  label: RubiConnect Webhooks API
  slug: rubiconnect-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/openapi/rubiconnect-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rubiconnect.com
  spf: true
hosts:
- cert_expires: Nov 12 00:30:49 2026 GMT
  host: console.rubiconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rubiconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RubiConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RubiConnect
provider_slug: rubiconnect
slug: rubiconnect-domain-security
source_filename: rubiconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.rubiconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 00:30:49 2026 GMT\n  hsts: false\ndomains:\n- domain: rubiconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubiconnect/refs/heads/main/security/rubiconnect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CPaaS
- Communications APIs
- Business Messaging
- RCS
- WhatsApp Business
- SMS
- Marketing & Campaigns
- Conversational AI
- MCP
- AI Agents
---
