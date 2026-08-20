---
api_specs:
- filename: dust-tt-agents-api-openapi.yml
  format: yaml
  label: Dust Agents API
  slug: dust-tt-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-agents-api-openapi.yml
- filename: dust-tt-apps-api-openapi.yml
  format: yaml
  label: Dust Apps API
  slug: dust-tt-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-apps-api-openapi.yml
- filename: dust-tt-conversations-api-openapi.yml
  format: yaml
  label: Dust Conversations API
  slug: dust-tt-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-conversations-api-openapi.yml
- filename: dust-tt-datasources-api-openapi.yml
  format: yaml
  label: Dust Datasources API
  slug: dust-tt-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-datasources-api-openapi.yml
- filename: dust-tt-datasourceviews-api-openapi.yml
  format: yaml
  label: Dust DatasourceViews API
  slug: dust-tt-datasourceviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-datasourceviews-api-openapi.yml
- filename: dust-tt-feedbacks-api-openapi.yml
  format: yaml
  label: Dust Feedbacks API
  slug: dust-tt-feedbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-feedbacks-api-openapi.yml
- filename: dust-tt-mcp-api-openapi.yml
  format: yaml
  label: Dust MCP API
  slug: dust-tt-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mcp-api-openapi.yml
- filename: dust-tt-mentions-api-openapi.yml
  format: yaml
  label: Dust Mentions API
  slug: dust-tt-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mentions-api-openapi.yml
- filename: dust-tt-search-api-openapi.yml
  format: yaml
  label: Dust Search API
  slug: dust-tt-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-search-api-openapi.yml
- filename: dust-tt-skills-api-openapi.yml
  format: yaml
  label: Dust Skills API
  slug: dust-tt-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-skills-api-openapi.yml
- filename: dust-tt-spaces-api-openapi.yml
  format: yaml
  label: Dust Spaces API
  slug: dust-tt-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-spaces-api-openapi.yml
- filename: dust-tt-tools-api-openapi.yml
  format: yaml
  label: Dust Tools API
  slug: dust-tt-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-tools-api-openapi.yml
- filename: dust-tt-triggers-api-openapi.yml
  format: yaml
  label: Dust Triggers API
  slug: dust-tt-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-triggers-api-openapi.yml
- filename: dust-tt-workspace-api-openapi.yml
  format: yaml
  label: Dust Workspace API
  slug: dust-tt-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dust.tt
  spf: true
hosts:
- cert_expires: Sep  5 12:39:29 2026 GMT
  host: dust.tt
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:26:33 2026 GMT
  host: docs.dust.tt
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 14:43:52 2026 GMT
  host: eu.dust.tt
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dust Tt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dust, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dust
provider_slug: dust-tt
slug: dust-tt-domain-security
source_filename: dust-tt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dust.tt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:39:29 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: docs.dust.tt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:26:33 2026 GMT\n  hsts: null\n- host: eu.dust.tt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: dust.tt\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/security/dust-tt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Artificial Intelligence
- Custom Workflows
- Data Sources
- Dust
- Enterprise AI
- Knowledge-Management
- LLM
- MCP
- Multi-Model
- RAG
---
