---
api_specs:
- filename: workato-data-tables-api-openapi.yml
  format: yaml
  label: Workato Data Tables API
  slug: workato-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-data-tables-api-openapi.yml
- filename: workato-genies-api-openapi.yml
  format: yaml
  label: Workato Genies API
  slug: workato-genies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-genies-api-openapi.yml
- filename: workato-knowledge-bases-api-openapi.yml
  format: yaml
  label: Workato Knowledge Bases API
  slug: workato-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-knowledge-bases-api-openapi.yml
- filename: workato-mcp-servers-api-openapi.yml
  format: yaml
  label: Workato MCP Servers API
  slug: workato-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-mcp-servers-api-openapi.yml
- filename: workato-messages-api-openapi.yml
  format: yaml
  label: Workato Messages API
  slug: workato-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-messages-api-openapi.yml
- filename: workato-policies-api-openapi.yml
  format: yaml
  label: Workato Policies API
  slug: workato-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-policies-api-openapi.yml
- filename: workato-recipes-api-openapi.yml
  format: yaml
  label: Workato Recipes API
  slug: workato-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-recipes-api-openapi.yml
- filename: workato-skills-api-openapi.yml
  format: yaml
  label: Workato Skills API
  slug: workato-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-skills-api-openapi.yml
- filename: workato-tools-api-openapi.yml
  format: yaml
  label: Workato Tools API
  slug: workato-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-tools-api-openapi.yml
- filename: workato-user-groups-api-openapi.yml
  format: yaml
  label: Workato User Groups API
  slug: workato-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workato/refs/heads/main/openapi/workato-user-groups-api-openapi.yml
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
