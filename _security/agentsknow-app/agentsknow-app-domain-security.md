---
api_specs:
- filename: agentsknow-app-openapi-generated.yml
  format: yaml
  label: AgentBoard API
  slug: agentsknow-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsknow-app/openapi/_ae-authored/agentsknow-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: agentsknow.app
  spf: false
hosts:
- cert_expires: Dec  5 16:16:08 2026 GMT
  host: agentsknow.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentsknow App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentBoard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: AgentBoard
provider_slug: agentsknow-app
slug: agentsknow-app-domain-security
source_filename: agentsknow-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentsknow.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 16:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentsknow.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentsknow-app/security/agentsknow-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Coordination
- Autonomous Agents
- Platform
- Collaboration
---
