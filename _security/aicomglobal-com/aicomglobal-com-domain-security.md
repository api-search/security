---
api_specs:
- filename: aicomglobal-com-agora-api-openapi.yml
  format: yaml
  label: aicomglobal Agora API
  slug: aicomglobal-com-agora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-agora-api-openapi.yml
- filename: aicomglobal-com-chronicle-api-openapi.yml
  format: yaml
  label: aicomglobal Chronicle API
  slug: aicomglobal-com-chronicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-chronicle-api-openapi.yml
- filename: aicomglobal-com-clear-api-openapi.yml
  format: yaml
  label: aicomglobal Clear API
  slug: aicomglobal-com-clear-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-clear-api-openapi.yml
- filename: aicomglobal-com-commons-api-openapi.yml
  format: yaml
  label: aicomglobal Commons API
  slug: aicomglobal-com-commons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-commons-api-openapi.yml
- filename: aicomglobal-com-discovery-api-openapi.yml
  format: yaml
  label: aicomglobal Discovery API
  slug: aicomglobal-com-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-discovery-api-openapi.yml
- filename: aicomglobal-com-join-api-openapi.yml
  format: yaml
  label: aicomglobal Join API
  slug: aicomglobal-com-join-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-join-api-openapi.yml
- filename: aicomglobal-com-oasis-api-openapi.yml
  format: yaml
  label: aicomglobal Oasis API
  slug: aicomglobal-com-oasis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-oasis-api-openapi.yml
- filename: aicomglobal-com-pulse-json-api-openapi.yml
  format: yaml
  label: aicomglobal Pulse.json API
  slug: aicomglobal-com-pulse-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-pulse-json-api-openapi.yml
- filename: aicomglobal-com-route-api-openapi.yml
  format: yaml
  label: aicomglobal Route API
  slug: aicomglobal-com-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-route-api-openapi.yml
- filename: aicomglobal-com-skill-md-api-openapi.yml
  format: yaml
  label: aicomglobal Skill.md API
  slug: aicomglobal-com-skill-md-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-skill-md-api-openapi.yml
- filename: aicomglobal-com-svc-api-openapi.yml
  format: yaml
  label: aicomglobal Svc API
  slug: aicomglobal-com-svc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-svc-api-openapi.yml
- filename: aicomglobal-com-verdict-api-openapi.yml
  format: yaml
  label: aicomglobal Verdict API
  slug: aicomglobal-com-verdict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-verdict-api-openapi.yml
- filename: aicomglobal-com-watch-api-openapi.yml
  format: yaml
  label: aicomglobal Watch API
  slug: aicomglobal-com-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-watch-api-openapi.yml
- filename: aicomglobal-com-x402-api-openapi.yml
  format: yaml
  label: aicomglobal X402 API
  slug: aicomglobal-com-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aicomglobal.com
  spf: false
hosts:
- cert_expires: Nov 14 00:40:18 2026 GMT
  host: aicomglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aicomglobal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aicomglobal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: aicomglobal
provider_slug: aicomglobal-com
slug: aicomglobal-com-domain-security
source_filename: aicomglobal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicomglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 00:40:18 2026 GMT\n  hsts: false\ndomains:\n- domain: aicomglobal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/security/aicomglobal-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Trust
- Reliability Monitoring
- Agent Discovery
- Agent Messaging
- Developer Tools
- Agent-Native
- United Kingdom
---
