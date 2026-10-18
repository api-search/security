---
api_specs:
- filename: beam-ai-agent-context-files-api-openapi.yml
  format: yaml
  label: Beam AI Agent Context Files API
  slug: beam-ai-agent-context-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-context-files-api-openapi.yml
- filename: beam-ai-agent-graph-api-openapi.yml
  format: yaml
  label: Beam AI Agent Graph API
  slug: beam-ai-agent-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-graph-api-openapi.yml
- filename: beam-ai-agent-setup-api-openapi.yml
  format: yaml
  label: Beam AI Agent Setup API
  slug: beam-ai-agent-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-setup-api-openapi.yml
- filename: beam-ai-agent-skills-api-openapi.yml
  format: yaml
  label: Beam AI Agent Skills API
  slug: beam-ai-agent-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-skills-api-openapi.yml
- filename: beam-ai-agent-task-api-openapi.yml
  format: yaml
  label: Beam AI Agent Task API
  slug: beam-ai-agent-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-task-api-openapi.yml
- filename: beam-ai-agent-views-api-openapi.yml
  format: yaml
  label: Beam AI Agent Views API
  slug: beam-ai-agent-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-views-api-openapi.yml
- filename: beam-ai-agents-api-openapi.yml
  format: yaml
  label: Beam AI Agents API
  slug: beam-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agents-api-openapi.yml
- filename: beam-ai-complete-agent-graph-api-openapi.yml
  format: yaml
  label: Beam AI Complete Agent Graph API
  slug: beam-ai-complete-agent-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-complete-agent-graph-api-openapi.yml
- filename: beam-ai-custom-tool-api-openapi.yml
  format: yaml
  label: Beam AI Custom Tool API
  slug: beam-ai-custom-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-custom-tool-api-openapi.yml
- filename: beam-ai-tool-api-openapi.yml
  format: yaml
  label: Beam AI Tool API
  slug: beam-ai-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-tool-api-openapi.yml
- filename: beam-ai-user-api-openapi.yml
  format: yaml
  label: Beam AI User API
  slug: beam-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beam.ai
  spf: true
hosts:
- cert_expires: Nov 26 03:19:47 2026 GMT
  host: beam.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beam Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beam AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beam AI
provider_slug: beam-ai
slug: beam-ai-domain-security
source_filename: beam-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 03:19:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/security/beam-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Enterprise
- Platform
---
