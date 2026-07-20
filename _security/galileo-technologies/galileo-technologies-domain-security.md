---
api_specs:
- filename: galileo-technologies-openapi-original.json
  format: json
  label: Galileo API
  slug: galileo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-technologies/refs/heads/main/openapi/galileo-technologies-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galileo.ai
  spf: true
hosts:
- cert_expires: Sep  8 11:42:58 2026 GMT
  host: api.galileo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galileo Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galileo Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galileo Technologies
provider_slug: galileo-technologies
slug: galileo-technologies-domain-security
source_filename: galileo-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:42:58 2026 GMT\n  hsts: null\ndomains:\n- domain: galileo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-technologies/refs/heads/main/security/galileo-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Observability
- LLM Evaluation
- Generative AI
- Agents
- Monitoring
- Machine Learning
- Guardrails
- Developer Tools
---
