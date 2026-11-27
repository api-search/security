---
api_specs:
- filename: algo-pw-agentcommons-api-api-openapi.yml
  format: yaml
  label: Agent Commons Agent Commons.Api API
  slug: algo-pw-agentcommons-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algo-pw/openapi/algo-pw-agentcommons-api-api-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: algo.pw
  spf: true
hosts:
- cert_expires: Jan  1 19:04:45 2027 GMT
  host: algo.pw
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Commons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Commons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Commons
provider_slug: algo-pw
slug: algo-pw-domain-security
source_filename: algo-pw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algo.pw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 19:04:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: algo.pw\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/algo-pw/security/algo-pw-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Agents
- Collaboration
- Evidence
- OpenAPI
- MCP
---
