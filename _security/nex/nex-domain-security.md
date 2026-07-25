---
api_specs:
- filename: nex-ai-lists-api-openapi.yml
  format: yaml
  label: Nex AI Lists API
  slug: nex-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-ai-lists-api-openapi.yml
- filename: nex-compounding-api-openapi.yml
  format: yaml
  label: Nex Compounding API
  slug: nex-compounding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-compounding-api-openapi.yml
- filename: nex-context-api-openapi.yml
  format: yaml
  label: Nex Context API
  slug: nex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-context-api-openapi.yml
- filename: nex-graph-api-openapi.yml
  format: yaml
  label: Nex Graph API
  slug: nex-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-graph-api-openapi.yml
- filename: nex-insights-api-openapi.yml
  format: yaml
  label: Nex Insights API
  slug: nex-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-insights-api-openapi.yml
- filename: nex-integrations-api-openapi.yml
  format: yaml
  label: Nex Integrations API
  slug: nex-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-integrations-api-openapi.yml
- filename: nex-lists-api-openapi.yml
  format: yaml
  label: Nex Lists API
  slug: nex-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-lists-api-openapi.yml
- filename: nex-notes-api-openapi.yml
  format: yaml
  label: Nex Notes API
  slug: nex-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notes-api-openapi.yml
- filename: nex-notifications-api-openapi.yml
  format: yaml
  label: Nex Notifications API
  slug: nex-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-notifications-api-openapi.yml
- filename: nex-objects-api-openapi.yml
  format: yaml
  label: Nex Objects API
  slug: nex-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-objects-api-openapi.yml
- filename: nex-records-api-openapi.yml
  format: yaml
  label: Nex Records API
  slug: nex-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-records-api-openapi.yml
- filename: nex-relationships-api-openapi.yml
  format: yaml
  label: Nex Relationships API
  slug: nex-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-relationships-api-openapi.yml
- filename: nex-schema-api-openapi.yml
  format: yaml
  label: Nex Schema API
  slug: nex-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-schema-api-openapi.yml
- filename: nex-search-api-openapi.yml
  format: yaml
  label: Nex Search API
  slug: nex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-search-api-openapi.yml
- filename: nex-tasks-api-openapi.yml
  format: yaml
  label: Nex Tasks API
  slug: nex-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-tasks-api-openapi.yml
- filename: nex-timeline-api-openapi.yml
  format: yaml
  label: Nex Timeline API
  slug: nex-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/openapi/nex-timeline-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@nex.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nex.ai
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: app.nex.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nex
provider_slug: nex
slug: nex-domain-security
source_filename: nex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.nex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nex.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@nex.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nex/refs/heads/main/security/nex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Knowledge Graph
- Context
- Memory
- MCP
- Model Context Protocol
- Workflow Automation
- Integrations
- Developer API
---
