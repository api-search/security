---
api_specs:
- filename: monaco-accounts-api-openapi.yml
  format: yaml
  label: Monaco Accounts API
  slug: monaco-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-accounts-api-openapi.yml
- filename: monaco-audiences-api-openapi.yml
  format: yaml
  label: Monaco Audiences API
  slug: monaco-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-audiences-api-openapi.yml
- filename: monaco-auth-api-openapi.yml
  format: yaml
  label: Monaco Auth API
  slug: monaco-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-auth-api-openapi.yml
- filename: monaco-campaigns-api-openapi.yml
  format: yaml
  label: Monaco Campaigns API
  slug: monaco-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-campaigns-api-openapi.yml
- filename: monaco-contacts-api-openapi.yml
  format: yaml
  label: Monaco Contacts API
  slug: monaco-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-contacts-api-openapi.yml
- filename: monaco-meetings-api-openapi.yml
  format: yaml
  label: Monaco Meetings API
  slug: monaco-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-meetings-api-openapi.yml
- filename: monaco-opportunities-api-openapi.yml
  format: yaml
  label: Monaco Opportunities API
  slug: monaco-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-opportunities-api-openapi.yml
- filename: monaco-schemas-api-openapi.yml
  format: yaml
  label: Monaco Schemas API
  slug: monaco-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-schemas-api-openapi.yml
- filename: monaco-sequence-templates-api-openapi.yml
  format: yaml
  label: Monaco Sequence Templates API
  slug: monaco-sequence-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequence-templates-api-openapi.yml
- filename: monaco-sequences-api-openapi.yml
  format: yaml
  label: Monaco Sequences API
  slug: monaco-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-sequences-api-openapi.yml
- filename: monaco-tags-api-openapi.yml
  format: yaml
  label: Monaco Tags API
  slug: monaco-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tags-api-openapi.yml
- filename: monaco-tasks-api-openapi.yml
  format: yaml
  label: Monaco Tasks API
  slug: monaco-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-tasks-api-openapi.yml
- filename: monaco-users-api-openapi.yml
  format: yaml
  label: Monaco Users API
  slug: monaco-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-users-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Monaco Trust Center
name_suffix: Trust Center
overview: Monaco maintains a public trust center covering its security and compliance posture.
provider_name: Monaco
provider_slug: monaco
slug: monaco-trust-center
source_filename: monaco-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.monaco.com\nsource: https://trust.monaco.com\nplatform: Vanta Trust Center\ncertifications: []\ncertifications_note: >-\n  The trust center is served by Vanta and renders entirely client-side; the\n  document returned to an unauthenticated HTTP fetch carries only the page shell\n  and Open Graph metadata. No named certification (SOC 2, ISO 27001, PCI DSS,\n  HIPAA, FedRAMP) was verifiable from the served HTML, and Vanta's trust-page\n  data endpoints are not anonymously readable. No `Compliance` pointer is emitted\n  in apis.yml until a named certification can be verified — the trust center is\n  recorded as present, not as evidence of a specific certification.\nlinked_from:\n- https://www.monaco.com (footer, \"Compliance & Trust\")\n- https://www.monaco.com/security\n- https://www.monaco.com/vulnerability-disclosure\nevidence:\n- source: https://trust.monaco.com\n  http_status: 200\n  content_type: text/html\n\
  \  signals: [<title>Monaco Trust Center</title>, 'meta keywords: Trust, Security, Compliance, Automation', assets.vanta.com]\n- source: https://trust.monaco.com/api/company\n  http_status: 200\n  note: Returns the SPA shell, not JSON — no machine-readable trust data.\nrelated:\n  vulnerability_disclosure: security/monaco-vulnerability-disclosure.yml\n  domain_security: security/monaco-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/security/monaco-trust-center.yml
summary_line: trust center published
tags:
- Company
- CRM
- Sales
- Revenue Operations
- Artificial Intelligence
- Contacts
- Account
- Opportunities
- Pipeline
- Go-To-Market
- MCP
- Campaigns
- Audiences
- Sales Engagement
- Agents
trust_url: https://trust.monaco.com
---
