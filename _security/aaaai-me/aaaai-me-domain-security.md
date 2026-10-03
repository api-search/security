---
api_specs:
- filename: aaaai-me-agents-api-openapi.yml
  format: yaml
  label: AAA AI Agents API
  slug: aaaai-me-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-agents-api-openapi.yml
- filename: aaaai-me-approvals-api-openapi.yml
  format: yaml
  label: AAA AI Approvals API
  slug: aaaai-me-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-approvals-api-openapi.yml
- filename: aaaai-me-auth-api-openapi.yml
  format: yaml
  label: AAA AI Auth API
  slug: aaaai-me-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-auth-api-openapi.yml
- filename: aaaai-me-chat-api-openapi.yml
  format: yaml
  label: AAA AI Chat API
  slug: aaaai-me-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-chat-api-openapi.yml
- filename: aaaai-me-code-api-openapi.yml
  format: yaml
  label: AAA AI Code API
  slug: aaaai-me-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-code-api-openapi.yml
- filename: aaaai-me-cognitive-scaling-api-openapi.yml
  format: yaml
  label: AAA AI Cognitive Scaling API
  slug: aaaai-me-cognitive-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-cognitive-scaling-api-openapi.yml
- filename: aaaai-me-cron-api-openapi.yml
  format: yaml
  label: AAA AI Cron API
  slug: aaaai-me-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-cron-api-openapi.yml
- filename: aaaai-me-debug-api-openapi.yml
  format: yaml
  label: AAA AI Debug API
  slug: aaaai-me-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-debug-api-openapi.yml
- filename: aaaai-me-deep-agent-api-openapi.yml
  format: yaml
  label: AAA AI Deep Agent API
  slug: aaaai-me-deep-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-deep-agent-api-openapi.yml
- filename: aaaai-me-dynamic-experts-api-openapi.yml
  format: yaml
  label: AAA AI Dynamic Experts API
  slug: aaaai-me-dynamic-experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-dynamic-experts-api-openapi.yml
- filename: aaaai-me-experts-api-openapi.yml
  format: yaml
  label: AAA AI Experts API
  slug: aaaai-me-experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-experts-api-openapi.yml
- filename: aaaai-me-health-api-openapi.yml
  format: yaml
  label: AAA AI Health API
  slug: aaaai-me-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-health-api-openapi.yml
- filename: aaaai-me-nodes-api-openapi.yml
  format: yaml
  label: AAA AI Nodes API
  slug: aaaai-me-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-nodes-api-openapi.yml
- filename: aaaai-me-settings-api-openapi.yml
  format: yaml
  label: AAA AI Settings API
  slug: aaaai-me-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-settings-api-openapi.yml
- filename: aaaai-me-user-api-openapi.yml
  format: yaml
  label: AAA AI User API
  slug: aaaai-me-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-user-api-openapi.yml
- filename: aaaai-me-video-api-openapi.yml
  format: yaml
  label: AAA AI Video API
  slug: aaaai-me-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aaaai.me
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: aaaai.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: web.aaaai.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aaaai Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAA AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AAA AI
provider_slug: aaaai-me
slug: aaaai-me-domain-security
source_filename: aaaai-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaaai.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n- host: web.aaaai.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aaaai.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/security/aaaai-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agents
- Multi-Agent
- LLM Orchestration
- Meetings
- Voice
- Video
- Workflows
- MCP
- Agentic Commerce
- OpenAI-Compatible
- Self-Hosted
- Agent-Native
- Montenegro
---
