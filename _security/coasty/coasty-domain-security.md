---
api_specs:
- filename: coasty-keys-api-openapi.yml
  format: yaml
  label: Coasty keys API
  slug: coasty-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-keys-api-openapi.yml
- filename: coasty-machines-api-openapi.yml
  format: yaml
  label: Coasty machines API
  slug: coasty-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-machines-api-openapi.yml
- filename: coasty-predict-api-openapi.yml
  format: yaml
  label: Coasty predict API
  slug: coasty-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-predict-api-openapi.yml
- filename: coasty-runs-api-openapi.yml
  format: yaml
  label: Coasty runs API
  slug: coasty-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-runs-api-openapi.yml
- filename: coasty-schedules-api-openapi.yml
  format: yaml
  label: Coasty schedules API
  slug: coasty-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-schedules-api-openapi.yml
- filename: coasty-sessions-api-openapi.yml
  format: yaml
  label: Coasty sessions API
  slug: coasty-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-sessions-api-openapi.yml
- filename: coasty-triggers-api-openapi.yml
  format: yaml
  label: Coasty triggers API
  slug: coasty-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-triggers-api-openapi.yml
- filename: coasty-workflows-api-openapi.yml
  format: yaml
  label: Coasty workflows API
  slug: coasty-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coasty/refs/heads/main/openapi/coasty-workflows-api-openapi.yml
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
