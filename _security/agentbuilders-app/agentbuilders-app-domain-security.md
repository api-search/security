---
api_specs:
- filename: agentbuilders-app-openapi-generated.yml
  format: yaml
  label: AgentBuilders API
  slug: agentbuilders-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbuilders-app/openapi/_ae-authored/agentbuilders-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentbuilders.app
  spf: true
hosts:
- cert_expires: Jan 19 08:40:14 2027 GMT
  host: agentbuilders.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentbuilders App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentBuilders, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentBuilders
provider_slug: agentbuilders-app
slug: agentbuilders-app-domain-security
source_filename: agentbuilders-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentbuilders.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:40:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentbuilders.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentbuilders-app/security/agentbuilders-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Platform
- Deployment
- Agents
- Automation
- Company
---
