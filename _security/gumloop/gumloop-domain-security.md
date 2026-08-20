---
api_specs:
- filename: gumloop-agents-api-openapi.yml
  format: yaml
  label: Gumloop Agents API
  slug: gumloop-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-agents-api-openapi.yml
- filename: gumloop-artifacts-api-openapi.yml
  format: yaml
  label: Gumloop Artifacts API
  slug: gumloop-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-artifacts-api-openapi.yml
- filename: gumloop-brain-api-openapi.yml
  format: yaml
  label: Gumloop Brain API
  slug: gumloop-brain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-brain-api-openapi.yml
- filename: gumloop-chat-completions-api-openapi.yml
  format: yaml
  label: Gumloop Chat completions API
  slug: gumloop-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-chat-completions-api-openapi.yml
- filename: gumloop-data-access-api-openapi.yml
  format: yaml
  label: Gumloop Data Access API
  slug: gumloop-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-data-access-api-openapi.yml
- filename: gumloop-evaluations-api-openapi.yml
  format: yaml
  label: Gumloop Evaluations API
  slug: gumloop-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-evaluations-api-openapi.yml
- filename: gumloop-execution-api-openapi.yml
  format: yaml
  label: Gumloop Execution API
  slug: gumloop-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-execution-api-openapi.yml
- filename: gumloop-file-handling-api-openapi.yml
  format: yaml
  label: Gumloop File Handling API
  slug: gumloop-file-handling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-file-handling-api-openapi.yml
- filename: gumloop-mcp-api-openapi.yml
  format: yaml
  label: Gumloop MCP API
  slug: gumloop-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-mcp-api-openapi.yml
- filename: gumloop-models-api-openapi.yml
  format: yaml
  label: Gumloop Models API
  slug: gumloop-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-models-api-openapi.yml
- filename: gumloop-organization-api-openapi.yml
  format: yaml
  label: Gumloop Organization API
  slug: gumloop-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-organization-api-openapi.yml
- filename: gumloop-sessions-api-openapi.yml
  format: yaml
  label: Gumloop Sessions API
  slug: gumloop-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-sessions-api-openapi.yml
- filename: gumloop-skills-api-openapi.yml
  format: yaml
  label: Gumloop Skills API
  slug: gumloop-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-skills-api-openapi.yml
- filename: gumloop-teams-api-openapi.yml
  format: yaml
  label: Gumloop Teams API
  slug: gumloop-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/openapi/gumloop-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gumloop.com
  spf: true
hosts:
- cert_expires: Aug 25 22:36:22 2026 GMT
  host: www.gumloop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:30:54 2026 GMT
  host: api.gumloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gumloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gumloop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gumloop
provider_slug: gumloop
slug: gumloop-domain-security
source_filename: gumloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gumloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:36:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gumloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:30:54 2026 GMT\n  hsts: null\ndomains:\n- domain: gumloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumloop/refs/heads/main/security/gumloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Automation
- Workflow-Automation
- Agent Platform
- MCP
- LLM
- No-Code
- Developer Tools
---
