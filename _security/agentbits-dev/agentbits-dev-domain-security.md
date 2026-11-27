---
api_specs:
- filename: agentbits-dev-health-api-openapi.yml
  format: yaml
  label: Agent Bits Health API
  slug: agentbits-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbits-dev/openapi/agentbits-dev-health-api-openapi.yml
- filename: agentbits-dev-tool-api-openapi.yml
  format: yaml
  label: Agent Bits Tool API
  slug: agentbits-dev-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbits-dev/openapi/agentbits-dev-tool-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentbits.dev
  spf: false
hosts:
- cert_expires: Jan  8 05:40:30 2027 GMT
  host: agentbits.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Bits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Bits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agent Bits
provider_slug: agentbits-dev
slug: agentbits-dev-domain-security
source_filename: agentbits-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentbits.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 05:40:30 2027 GMT\n  hsts: false\ndomains:\n- domain: agentbits.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentbits-dev/security/agentbits-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Utilities
- Data
- Tools
- Machine-Readable
---
