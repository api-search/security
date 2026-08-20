---
api_specs:
- filename: truto-accounts-api-openapi.yml
  format: yaml
  label: Truto Accounts API
  slug: truto-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-accounts-api-openapi.yml
- filename: truto-applications-api-openapi.yml
  format: yaml
  label: Truto Applications API
  slug: truto-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-applications-api-openapi.yml
- filename: truto-candidates-api-openapi.yml
  format: yaml
  label: Truto Candidates API
  slug: truto-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-candidates-api-openapi.yml
- filename: truto-companies-api-openapi.yml
  format: yaml
  label: Truto Companies API
  slug: truto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-companies-api-openapi.yml
- filename: truto-contacts-api-openapi.yml
  format: yaml
  label: Truto Contacts API
  slug: truto-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-contacts-api-openapi.yml
- filename: truto-departments-api-openapi.yml
  format: yaml
  label: Truto Departments API
  slug: truto-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-departments-api-openapi.yml
- filename: truto-employees-api-openapi.yml
  format: yaml
  label: Truto Employees API
  slug: truto-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-employees-api-openapi.yml
- filename: truto-employments-api-openapi.yml
  format: yaml
  label: Truto Employments API
  slug: truto-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-employments-api-openapi.yml
- filename: truto-groups-api-openapi.yml
  format: yaml
  label: Truto Groups API
  slug: truto-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-groups-api-openapi.yml
- filename: truto-integrated-accounts-api-openapi.yml
  format: yaml
  label: Truto Integrated Accounts API
  slug: truto-integrated-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-integrated-accounts-api-openapi.yml
- filename: truto-jobs-api-openapi.yml
  format: yaml
  label: Truto Jobs API
  slug: truto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-jobs-api-openapi.yml
- filename: truto-link-tokens-api-openapi.yml
  format: yaml
  label: Truto Link Tokens API
  slug: truto-link-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-link-tokens-api-openapi.yml
- filename: truto-mcp-servers-api-openapi.yml
  format: yaml
  label: Truto MCP Servers API
  slug: truto-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-mcp-servers-api-openapi.yml
- filename: truto-offers-api-openapi.yml
  format: yaml
  label: Truto Offers API
  slug: truto-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-offers-api-openapi.yml
- filename: truto-opportunities-api-openapi.yml
  format: yaml
  label: Truto Opportunities API
  slug: truto-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-opportunities-api-openapi.yml
- filename: truto-stages-api-openapi.yml
  format: yaml
  label: Truto Stages API
  slug: truto-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-stages-api-openapi.yml
- filename: truto-tasks-api-openapi.yml
  format: yaml
  label: Truto Tasks API
  slug: truto-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-tasks-api-openapi.yml
- filename: truto-timeoff-api-openapi.yml
  format: yaml
  label: Truto Timeoff API
  slug: truto-timeoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-timeoff-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: truto.one
  spf: true
hosts:
- cert_expires: Oct  5 22:00:49 2026 GMT
  host: truto.one
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 12:16:56 2026 GMT
  host: api.truto.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Truto
provider_slug: truto
slug: truto-domain-security
source_filename: truto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truto.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.truto.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:16:56 2026 GMT\n  hsts: null\ndomains:\n- domain: truto.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/security/truto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Unified-API
- Integration Platform
- HRIS
- ATS
- CRM
- Embedded Integrations
- MCP
- AI Agents
- Software-as-a-Service
---
