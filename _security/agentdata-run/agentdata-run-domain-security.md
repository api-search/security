---
api_specs:
- filename: agentdata-run-openapi-generated.yml
  format: yaml
  label: AgentData API
  slug: agentdata-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdata-run/openapi/_ae-authored/agentdata-run-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentdata.run
  spf: true
hosts:
- cert_expires: Jan  7 18:13:57 2027 GMT
  host: agentdata.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentdata Run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgentData
provider_slug: agentdata-run
slug: agentdata-run-domain-security
source_filename: agentdata-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdata.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 18:13:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentdata.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentdata-run/security/agentdata-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
