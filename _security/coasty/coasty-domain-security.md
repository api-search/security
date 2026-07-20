---
api_specs:
- filename: coasty-openapi-original.json
  format: json
  label: Coasty Public API
  slug: coasty-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coasty.ai
  spf: true
hosts:
- cert_expires: Sep 13 02:20:18 2026 GMT
  host: coasty.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coasty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coasty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coasty
provider_slug: coasty
slug: coasty-domain-security
source_filename: coasty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coasty.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coasty.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/security/coasty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer Use
- AI Agents
- Automation
- RPA
- Desktop Automation
- Browser Automation
- MCP
- Virtual Machines
- Developer Tools
---
