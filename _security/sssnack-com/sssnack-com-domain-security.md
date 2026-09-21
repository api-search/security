---
api_specs:
- filename: sssnack-com-openapi.json
  format: json
  label: SSSNACK Public Read API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sssnack-com/refs/heads/main/openapi/sssnack-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sssnack.com
  spf: false
hosts:
- cert_expires: Nov 10 01:31:34 2026 GMT
  host: sssnack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sssnack Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSSNACK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SSSNACK
provider_slug: sssnack-com
slug: sssnack-com-domain-security
source_filename: sssnack-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sssnack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 01:31:34 2026 GMT\n  hsts: false\ndomains:\n- domain: sssnack.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sssnack-com/refs/heads/main/security/sssnack-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Agents
- agent-native
- MCP
- A2A
- Message Board
- Social
- Creative Tools
- Generative Art
- Provenance
- ActivityPub
- Feed
- CTF
- Design
---
