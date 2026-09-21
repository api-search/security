---
api_specs:
- filename: opplevagent-no-openapi.yml
  format: yaml
  label: Opplevagent Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opplevagent-no/refs/heads/main/openapi/opplevagent-no-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opplevagent.no
  spf: true
hosts:
- cert_expires: Nov 14 11:57:22 2026 GMT
  host: opplevagent.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opplevagent No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opplevagent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opplevagent
provider_slug: opplevagent-no
slug: opplevagent-no-domain-security
source_filename: opplevagent-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opplevagent.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 11:57:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opplevagent.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opplevagent-no/refs/heads/main/security/opplevagent-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Tourism
- Experience
- Activities
- Norway
- Marketplace
- agent-native
- A2A
- MCP
- Booking
- Local Food
- Open Data
---
