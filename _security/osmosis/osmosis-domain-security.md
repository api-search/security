---
api_specs:
- filename: osmosis-agent-api-openapi.yml
  format: yaml
  label: Osmosis agent API
  slug: osmosis-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/openapi/osmosis-agent-api-openapi.yml
- filename: osmosis-knowledge-api-openapi.yml
  format: yaml
  label: Osmosis knowledge API
  slug: osmosis-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/openapi/osmosis-knowledge-api-openapi.yml
- filename: osmosis-osmosis-agent-improvement-api-api-openapi.yml
  format: yaml
  label: Osmosis Osmosis Agent Improvement API API
  slug: osmosis-osmosis-agent-improvement-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/openapi/osmosis-osmosis-agent-improvement-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: osmosis.ai
  spf: true
hosts:
- cert_expires: Aug 30 11:44:01 2026 GMT
  host: osmosis.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmosis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osmosis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Osmosis
provider_slug: osmosis
slug: osmosis-domain-security
source_filename: osmosis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osmosis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:44:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osmosis.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmosis/refs/heads/main/security/osmosis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Reinforcement Learning
- LLM
- Post-Training
- Model Training
- Agents
- Machine-Learning
- Developer Tools
---
