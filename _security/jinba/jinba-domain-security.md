---
api_specs:
- filename: jinba-api-keys-api-openapi.yml
  format: yaml
  label: Jinba API Keys API
  slug: jinba-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-api-keys-api-openapi.yml
- filename: jinba-credits-api-openapi.yml
  format: yaml
  label: Jinba Credits API
  slug: jinba-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-credits-api-openapi.yml
- filename: jinba-execution-api-openapi.yml
  format: yaml
  label: Jinba Execution API
  slug: jinba-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-execution-api-openapi.yml
- filename: jinba-explore-api-openapi.yml
  format: yaml
  label: Jinba Explore API
  slug: jinba-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-explore-api-openapi.yml
- filename: jinba-flows-api-openapi.yml
  format: yaml
  label: Jinba Flows API
  slug: jinba-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-flows-api-openapi.yml
- filename: jinba-mcp-api-openapi.yml
  format: yaml
  label: Jinba MCP API
  slug: jinba-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-mcp-api-openapi.yml
- filename: jinba-members-api-openapi.yml
  format: yaml
  label: Jinba Members API
  slug: jinba-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-members-api-openapi.yml
- filename: jinba-organizations-api-openapi.yml
  format: yaml
  label: Jinba Organizations API
  slug: jinba-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-organizations-api-openapi.yml
- filename: jinba-public-api-openapi.yml
  format: yaml
  label: Jinba Public API
  slug: jinba-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-public-api-openapi.yml
- filename: jinba-runs-api-openapi.yml
  format: yaml
  label: Jinba Runs API
  slug: jinba-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-runs-api-openapi.yml
- filename: jinba-tools-api-openapi.yml
  format: yaml
  label: Jinba Tools API
  slug: jinba-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-tools-api-openapi.yml
- filename: jinba-toolsets-api-openapi.yml
  format: yaml
  label: Jinba ToolSets API
  slug: jinba-toolsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-toolsets-api-openapi.yml
- filename: jinba-versions-api-openapi.yml
  format: yaml
  label: Jinba Versions API
  slug: jinba-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-versions-api-openapi.yml
- filename: jinba-webhooks-api-openapi.yml
  format: yaml
  label: Jinba Webhooks API
  slug: jinba-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/openapi/jinba-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jinba.io
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: jinba.dev
  spf: false
hosts:
- host: docs.jinba.io
  https: false
- cert_expires: Aug 28 16:24:04 2026 GMT
  host: toolbox-api.jinba.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 21:47:49 2026 GMT
  host: api.jinba.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jinba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jinba, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Jinba
provider_slug: jinba
slug: jinba-domain-security
source_filename: jinba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.jinba.io\n  https: false\n- host: toolbox-api.jinba.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:24:04 2026 GMT\n  hsts: null\n- host: api.jinba.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:47:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jinba.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: jinba.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jinba/refs/heads/main/security/jinba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Agents
- Workflow-Automation
- Enterprise
- MCP
- Low-Code
- Developer Tools
- Tools
- Automation
---
