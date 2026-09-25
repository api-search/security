---
api_specs:
- filename: wrongbeauty-com-swarm-api-openapi.yml
  format: yaml
  label: THE SWARM API
  slug: the-swarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wrongbeauty-com/refs/heads/main/openapi/wrongbeauty-com-swarm-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wrongbeauty.com
  spf: true
hosts:
- cert_expires: Dec 14 19:07:22 2026 GMT
  host: wrongbeauty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 15:09:50 2026 GMT
  host: swarm-api.wrongbeauty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wrongbeauty Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WRONG BEAUTY 000 / THE SWARM, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WRONG BEAUTY 000 / THE SWARM
provider_slug: wrongbeauty-com
slug: wrongbeauty-com-domain-security
source_filename: wrongbeauty-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wrongbeauty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 19:07:22 2026 GMT\n  hsts: false\n- host: swarm-api.wrongbeauty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:09:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wrongbeauty.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrongbeauty-com/refs/heads/main/security/wrongbeauty-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Art
- Exhibitions
- Agents
- A2A
- Agent-Native
- Curation
- Provenance
- Ledger
- Culture
- Italy
---
