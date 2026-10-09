---
api_specs:
- filename: tale-dev-agents-api-openapi.yml
  format: yaml
  label: Tale Agents API
  slug: tale-dev-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-agents-api-openapi.yml
- filename: tale-dev-automations-api-openapi.yml
  format: yaml
  label: Tale Automations API
  slug: tale-dev-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-automations-api-openapi.yml
- filename: tale-dev-browser-sessions-api-openapi.yml
  format: yaml
  label: Tale Browser sessions API
  slug: tale-dev-browser-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-browser-sessions-api-openapi.yml
- filename: tale-dev-contacts-api-openapi.yml
  format: yaml
  label: Tale Contacts API
  slug: tale-dev-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-contacts-api-openapi.yml
- filename: tale-dev-conversations-api-openapi.yml
  format: yaml
  label: Tale Conversations API
  slug: tale-dev-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-conversations-api-openapi.yml
- filename: tale-dev-documents-api-openapi.yml
  format: yaml
  label: Tale Documents API
  slug: tale-dev-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-documents-api-openapi.yml
- filename: tale-dev-knowledge-api-openapi.yml
  format: yaml
  label: Tale Knowledge API
  slug: tale-dev-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-knowledge-api-openapi.yml
- filename: tale-dev-mcp-api-openapi.yml
  format: yaml
  label: Tale MCP API
  slug: tale-dev-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-mcp-api-openapi.yml
- filename: tale-dev-model-endpoints-api-openapi.yml
  format: yaml
  label: Tale Model endpoints API
  slug: tale-dev-model-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-model-endpoints-api-openapi.yml
- filename: tale-dev-notifications-api-openapi.yml
  format: yaml
  label: Tale Notifications API
  slug: tale-dev-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-notifications-api-openapi.yml
- filename: tale-dev-organization-api-openapi.yml
  format: yaml
  label: Tale Organization API
  slug: tale-dev-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-organization-api-openapi.yml
- filename: tale-dev-products-api-openapi.yml
  format: yaml
  label: Tale Products API
  slug: tale-dev-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-products-api-openapi.yml
- filename: tale-dev-projects-api-openapi.yml
  format: yaml
  label: Tale Projects API
  slug: tale-dev-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-projects-api-openapi.yml
- filename: tale-dev-runs-api-openapi.yml
  format: yaml
  label: Tale Runs API
  slug: tale-dev-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-runs-api-openapi.yml
- filename: tale-dev-skills-api-openapi.yml
  format: yaml
  label: Tale Skills API
  slug: tale-dev-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-skills-api-openapi.yml
- filename: tale-dev-tasks-api-openapi.yml
  format: yaml
  label: Tale Tasks API
  slug: tale-dev-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-tasks-api-openapi.yml
- filename: tale-dev-threads-api-openapi.yml
  format: yaml
  label: Tale Threads API
  slug: tale-dev-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-threads-api-openapi.yml
- filename: tale-dev-websites-api-openapi.yml
  format: yaml
  label: Tale Websites API
  slug: tale-dev-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-websites-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tale.dev
  spf: true
hosts:
- cert_expires: Dec 31 20:48:22 2026 GMT
  host: tale.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tale Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tale
provider_slug: tale-dev
slug: tale-dev-domain-security
source_filename: tale-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tale.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 20:48:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tale.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/security/tale-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Agents
- Automation
- Knowledge Management
- MCP
- Open Source
- Self-Hosted
---
