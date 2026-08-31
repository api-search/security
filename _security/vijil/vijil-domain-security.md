---
api_specs:
- filename: vijil-agent-environment-api-openapi.yml
  format: yaml
  label: Vijil Agent Environment API
  slug: vijil-agent-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-agent-environment-api-openapi.yml
- filename: vijil-diamond-api-openapi.yml
  format: yaml
  label: Vijil Diamond API
  slug: vijil-diamond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-diamond-api-openapi.yml
- filename: vijil-dome-api-openapi.yml
  format: yaml
  label: Vijil Dome API
  slug: vijil-dome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-dome-api-openapi.yml
- filename: vijil-red-team-api-openapi.yml
  format: yaml
  label: Vijil Red Team API
  slug: vijil-red-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-red-team-api-openapi.yml
- filename: vijil-teams-api-openapi.yml
  format: yaml
  label: Vijil Teams API
  slug: vijil-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/openapi/vijil-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vijil.ai
  spf: true
hosts:
- cert_expires: Sep 13 19:38:58 2026 GMT
  host: vijil.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vijil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vijil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vijil
provider_slug: vijil
slug: vijil-domain-security
source_filename: vijil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vijil.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:38:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vijil.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vijil/refs/heads/main/security/vijil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Security
- AI Safety
- Trust
- Red Teaming
- Guardrails
- LLM Security
- Evaluation
- Observability
- MCP
---
