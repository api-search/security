---
api_specs:
- filename: agentskit-io-openapi-generated.yml
  format: yaml
  label: AgentsKit API
  slug: agentskit-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentskit-io/openapi/_ae-authored/agentskit-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentskit.io
  spf: true
hosts:
- cert_expires: Jan 11 13:13:01 2027 GMT
  host: agentskit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgentsKit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentsKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AgentsKit
provider_slug: agentskit-io
slug: agentskit-io-domain-security
source_filename: agentskit-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentskit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 13:13:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentskit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentskit-io/security/agentskit-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Agents
- TypeScript
- Platform
- LLM
---
