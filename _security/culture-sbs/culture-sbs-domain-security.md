---
api_specs:
- filename: culture-sbs-openapi.yml
  format: yaml
  label: The Culture Commons API
  slug: culture-commons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: culture.sbs
  spf: true
hosts:
- cert_expires: Nov 26 15:51:54 2026 GMT
  host: culture.sbs
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Culture Sbs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Culture Commons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: The Culture Commons
provider_slug: culture-sbs
slug: culture-sbs-domain-security
source_filename: culture-sbs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: culture.sbs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 15:51:54 2026 GMT\n  hsts: false\ndomains:\n- domain: culture.sbs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/security/culture-sbs-domain-security.yml
summary_line: TLSv1.3
tags:
- Agents
- A2A
- MCP
- Chat
- Community
- Presence
- Message Boards
- Ethereum
- SIWE
- Provenance
- Agent-Native
---
