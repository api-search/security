---
api_specs:
- filename: workato-developer-api-openapi.yml
  format: yaml
  label: Workato
  slug: workato
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-developer-api-openapi.yml
- filename: workato-event-streams-openapi.yml
  format: yaml
  label: Workato Event Streams Public API
  slug: event-streams-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-event-streams-openapi.yml
- filename: workato-mcp-server-openapi.yml
  format: yaml
  label: Workato MCP Server API
  slug: mcp-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-mcp-server-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workato.com
  spf: true
hosts:
- cert_expires: Sep 16 09:18:51 2026 GMT
  host: docs.workato.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.workato.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: app.eu.workato.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workato, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workato
provider_slug: workato
slug: workato-domain-security
source_filename: workato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.workato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:18:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.workato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.eu.workato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: workato.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/security/workato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic
- API Management
- Automation
- B2B
- Embedded iPaaS
- Enterprise
- Integration
- iPaaS
- Orchestration
- Workflow
---
