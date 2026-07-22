---
api_specs:
- filename: the-interaction-company-of-california-poke-openapi.yml
  format: yaml
  label: Poke API
  slug: poke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-interaction-company-of-california/refs/heads/main/openapi/the-interaction-company-of-california-poke-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: poke.com
  spf: true
hosts:
- cert_expires: Aug 24 09:17:06 2026 GMT
  host: poke.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Interaction Company Of California Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Interaction Company Of California, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Interaction Company Of California
provider_slug: the-interaction-company-of-california
slug: the-interaction-company-of-california-domain-security
source_filename: the-interaction-company-of-california-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:17:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: poke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-interaction-company-of-california/refs/heads/main/security/the-interaction-company-of-california-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Assistant
- Artificial Intelligence
- Agents
- Messaging
- Model Context Protocol
- MCP
- Productivity
- Automation
- Conversational AI
---
