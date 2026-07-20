---
api_specs:
- filename: jinba-toolbox-openapi.yml
  format: yaml
  label: Jinba Toolbox API
  slug: jinba-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-toolbox-openapi.yml
- filename: jinba-flow-openapi.yml
  format: yaml
  label: Jinba Flow External API
  slug: jinba-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-flow-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jinba.io
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: jinba.dev
  spf: false
hosts:
- host: docs.jinba.io
  https: false
- cert_expires: Aug 28 16:24:04 2026 GMT
  host: toolbox-api.jinba.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 21:47:49 2026 GMT
  host: api.jinba.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jinba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jinba, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Jinba
provider_slug: jinba
slug: jinba-domain-security
source_filename: jinba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.jinba.io\n  https: false\n- host: toolbox-api.jinba.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:24:04 2026 GMT\n  hsts: null\n- host: api.jinba.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:47:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jinba.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: jinba.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/security/jinba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- AI
- Agents
- Workflow Automation
- Enterprise
- MCP
- Low-Code
- Developer Tools
- Tools
- Automation
---
