---
api_specs:
- filename: cogny-openapi.yml
  format: yaml
  label: Cogny API
  slug: cogny-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cogny.com
  spf: true
hosts:
- cert_expires: Sep  1 00:40:05 2026 GMT
  host: api.cogny.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cogny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cogny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cogny
provider_slug: cogny
slug: cogny-domain-security
source_filename: cogny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cogny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:40:05 2026 GMT\n  hsts: null\ndomains:\n- domain: cogny.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/security/cogny-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
---
