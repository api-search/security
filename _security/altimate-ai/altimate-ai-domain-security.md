---
api_specs:
- filename: altimate-ai-openapi-original.json
  format: json
  label: Altimate AI Platform API
  slug: altimate-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/openapi/altimate-ai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: altimate.ai
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: altimate.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altimate Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altimate AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Altimate AI
provider_slug: altimate-ai
slug: altimate-ai-domain-security
source_filename: altimate-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altimate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: altimate.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altimate-ai/refs/heads/main/security/altimate-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Data Engineering
- Artificial Intelligence
- Agents
- MCP
- dbt
- Data Governance
- Data Contracts
- Analytics Engineering
---
