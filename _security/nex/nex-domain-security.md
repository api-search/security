---
api_specs:
- filename: nex-openapi-original.json
  format: json
  label: Nex Developer API
  slug: nex-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@nex.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nex.ai
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: app.nex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nex
provider_slug: nex
slug: nex-domain-security
source_filename: nex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.nex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nex.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@nex.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/security/nex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Knowledge Graph
- Context
- Memory
- MCP
- Model Context Protocol
- Workflow Automation
- Integrations
- Developer API
---
