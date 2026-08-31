---
api_specs:
- filename: toolhouse-agent-runs-api-openapi.yml
  format: yaml
  label: Toolhouse Agent Runs API
  slug: toolhouse-agent-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-agent-runs-api-openapi.yml
- filename: toolhouse-api-keys-api-openapi.yml
  format: yaml
  label: Toolhouse API Keys API
  slug: toolhouse-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-api-keys-api-openapi.yml
- filename: toolhouse-backoffice-api-openapi.yml
  format: yaml
  label: Toolhouse Backoffice API
  slug: toolhouse-backoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-backoffice-api-openapi.yml
- filename: toolhouse-logs-api-openapi.yml
  format: yaml
  label: Toolhouse Logs API
  slug: toolhouse-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-logs-api-openapi.yml
- filename: toolhouse-metrics-api-openapi.yml
  format: yaml
  label: Toolhouse Metrics API
  slug: toolhouse-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-metrics-api-openapi.yml
- filename: toolhouse-sdk-api-api-openapi.yml
  format: yaml
  label: Toolhouse SDK API API
  slug: toolhouse-sdk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-sdk-api-api-openapi.yml
- filename: toolhouse-user-api-api-openapi.yml
  format: yaml
  label: Toolhouse User API API
  slug: toolhouse-user-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/openapi/toolhouse-user-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toolhouse.ai
  spf: true
hosts:
- cert_expires: Sep 28 22:59:59 2026 GMT
  host: toolhouse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:23:34 2026 GMT
  host: docs.toolhouse.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 21:53:14 2026 GMT
  host: agents.toolhouse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toolhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toolhouse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Toolhouse
provider_slug: toolhouse
slug: toolhouse-domain-security
source_filename: toolhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toolhouse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:59:59 2026 GMT\n  hsts: false\n- host: docs.toolhouse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agents.toolhouse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:53:14 2026 GMT\n  hsts: false\ndomains:\n- domain: toolhouse.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toolhouse/refs/heads/main/security/toolhouse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Infrastructure
- AI Agents
- AI Workers
- Backend as a Service
- MCP
- MCP Discovery
- RAG
- Tools
- Workers API
---
