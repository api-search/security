---
api_specs:
- filename: agentsim-dev-agents-api-openapi.yml
  format: yaml
  label: AgentSIM Agents API
  slug: agentsim-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-agents-api-openapi.yml
- filename: agentsim-dev-browser-access-api-openapi.yml
  format: yaml
  label: AgentSIM Browser Access API
  slug: agentsim-dev-browser-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-browser-access-api-openapi.yml
- filename: agentsim-dev-sessions-api-openapi.yml
  format: yaml
  label: AgentSIM Sessions API
  slug: agentsim-dev-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: agentsim.dev
  spf: true
hosts:
- cert_expires: Dec 14 07:59:37 2026 GMT
  host: agentsim.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentsim Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentSIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AgentSIM
provider_slug: agentsim-dev
slug: agentsim-dev-domain-security
source_filename: agentsim-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentsim.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 07:59:37 2026 GMT\n  hsts: false\ndomains:\n- domain: agentsim.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentsim-dev/security/agentsim-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AgentSIM
- Authentication
- Identity
- Security
---
