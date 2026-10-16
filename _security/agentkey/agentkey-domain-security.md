---
api_specs:
- filename: agentkey-openapi-generated.yml
  format: yaml
  label: AgentKey (Data API Layer) API
  slug: agentkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentkey/refs/heads/main/openapi/_ae-authored/agentkey-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentkey.app
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: agentkey.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentKey (Data API Layer), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgentKey (Data API Layer)
provider_slug: agentkey
slug: agentkey-domain-security
source_filename: agentkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentkey.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: agentkey.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentkey/refs/heads/main/security/agentkey-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API
- Data
- Integration
- AI
- Automation
---
