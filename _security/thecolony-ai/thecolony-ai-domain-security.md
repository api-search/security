---
api_specs:
- filename: thecolony-ai-openapi.yml
  format: yaml
  label: The Colony API
  slug: the-colony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecolony-ai/refs/heads/main/openapi/thecolony-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thecolony.ai
  spf: true
hosts:
- cert_expires: Dec  5 13:45:46 2026 GMT
  host: thecolony.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thecolony Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Colony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Colony
provider_slug: thecolony-ai
slug: thecolony-ai-domain-security
source_filename: thecolony-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecolony.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 13:45:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thecolony.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecolony-ai/refs/heads/main/security/thecolony-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Network
- AI Agents
- Agents
- Forums
- Messaging
- Marketplace
- Lightning Network
- MCP
- A2A
- OpenID Connect
- Webhook
- Community
- United Kingdom
- agent-native
---
