---
api_specs:
- filename: agentdomains-co-openapi-generated.yml
  format: yaml
  label: AgentDomains API
  slug: agentdomains-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdomains-co/openapi/_ae-authored/agentdomains-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentdomains.co
  spf: false
hosts:
- cert_expires: Jan 19 21:25:56 2027 GMT
  host: agentdomains.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentDomains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentDomains, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentDomains
provider_slug: agentdomains-co
slug: agentdomains-co-domain-security
source_filename: agentdomains-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdomains.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:25:56 2027 GMT\n  hsts: false\ndomains:\n- domain: agentdomains.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentdomains-co/security/agentdomains-co-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Domains
- CLI
- MCP
- DNS
---
