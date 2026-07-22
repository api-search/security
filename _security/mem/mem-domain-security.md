---
api_specs:
- filename: mem-openapi-original.json
  format: json
  label: Mem Public Client API
  slug: mem-public-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/openapi/mem-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mem.ai
  spf: true
hosts:
- cert_expires: Oct 16 04:49:03 2026 GMT
  host: api.mem.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mem
provider_slug: mem
slug: mem-domain-security
source_filename: mem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:49:03 2026 GMT\n  hsts: null\ndomains:\n- domain: mem.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/security/mem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Notes
- Knowledge Management
- Productivity
- Artificial Intelligence
- Note Taking
- Search
- MCP
- Agents
- Meetings
---
