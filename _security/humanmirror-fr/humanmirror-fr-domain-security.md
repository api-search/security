---
api_specs:
- filename: humanmirror-fr-x402-openapi.yml
  format: yaml
  label: HumanMirror X402 API
  slug: x402
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-x402-openapi.yml
- filename: humanmirror-fr-sanitize-shield-openapi.yml
  format: yaml
  label: HumanMirror M2M Core Services
  slug: m2m-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-sanitize-shield-openapi.yml
- filename: humanmirror-fr-oracle-openapi.yml
  format: yaml
  label: HumanMirror Oracle API
  slug: oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-oracle-openapi.yml
- filename: humanmirror-fr-forge-openapi.yml
  format: yaml
  label: HumanMirror Forge API
  slug: forge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-forge-openapi.yml
- filename: humanmirror-fr-nexus-openapi.yml
  format: yaml
  label: HumanMirror Nexus API
  slug: nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-nexus-openapi.yml
- filename: humanmirror-fr-agentops-openapi.yml
  format: yaml
  label: HumanMirror AgentOps API
  slug: agentops
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-agentops-openapi.yml
- filename: humanmirror-fr-magnet-openapi.yml
  format: yaml
  label: HumanMirror Magnet API
  slug: magnet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-magnet-openapi.yml
- filename: humanmirror-fr-outcome-openapi.yml
  format: yaml
  label: HumanMirror Outcome API
  slug: outcome
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-outcome-openapi.yml
- filename: humanmirror-fr-one-openapi.yml
  format: yaml
  label: HumanMirror One API
  slug: one
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-one-openapi.yml
- filename: humanmirror-fr-flow-openapi.yml
  format: yaml
  label: HumanMirror Flow API
  slug: flow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-flow-openapi.yml
- filename: humanmirror-fr-market-openapi.yml
  format: yaml
  label: HumanMirror Intent Market API
  slug: market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-market-openapi.yml
- filename: humanmirror-fr-agent-os-openapi.yml
  format: yaml
  label: HumanMirror Agent OS API
  slug: agent-os
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-agent-os-openapi.yml
- filename: humanmirror-fr-physical-oracle-openapi.yml
  format: yaml
  label: HumanMirror Physical Oracle API
  slug: physical-oracle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-physical-oracle-openapi.yml
- filename: humanmirror-fr-automata-openapi.yml
  format: yaml
  label: HumanMirror Automata API
  slug: automata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/openapi/humanmirror-fr-automata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: humanmirror.fr
  spf: true
hosts:
- cert_expires: Nov 21 07:52:26 2026 GMT
  host: humanmirror.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Humanmirror Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanMirror, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: HumanMirror
provider_slug: humanmirror-fr
slug: humanmirror-fr-domain-security
source_filename: humanmirror-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanmirror.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:52:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humanmirror.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanmirror-fr/refs/heads/main/security/humanmirror-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI Agents
- Agent Security
- Prompt Injection Defense
- x402
- Machine Payments
- USDC
- MCP
- A2A
- Data Quality
- Verified Outcomes
- Microtransactions
- France
---
