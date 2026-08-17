---
api_specs:
- filename: fullcontact-address-api-openapi.yml
  format: yaml
  label: FullContact Address API
  slug: fullcontact-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-address-api-openapi.yml
- filename: fullcontact-audience-api-openapi.yml
  format: yaml
  label: FullContact Audience API
  slug: fullcontact-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-audience-api-openapi.yml
- filename: fullcontact-enrich-api-openapi.yml
  format: yaml
  label: FullContact Enrich API
  slug: fullcontact-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-enrich-api-openapi.yml
- filename: fullcontact-identity-api-openapi.yml
  format: yaml
  label: FullContact Identity API
  slug: fullcontact-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-identity-api-openapi.yml
- filename: fullcontact-permission-api-openapi.yml
  format: yaml
  label: FullContact Permission API
  slug: fullcontact-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-permission-api-openapi.yml
- filename: fullcontact-tags-api-openapi.yml
  format: yaml
  label: FullContact Tags API
  slug: fullcontact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/openapi/fullcontact-tags-api-openapi.yml
certifications:
- SOC 2
description: FullContact runs a Vanta-hosted Trust Center at trust.fullcontact.com. The page returns 200 but is a client-side rendered single-page app, so its certification list is not machine-readable from the served HTML. The one certification FullContact names in plain text in its own documentation is SOC 2, and that is the only one recorded here.
kind: trust-center
layout: security
name: Fullcontact Trust Center
name_suffix: Trust Center
overview: FullContact maintains a public trust center documenting SOC 2 compliance.
provider_name: FullContact
provider_slug: fullcontact
slug: fullcontact-trust-center
source_filename: fullcontact-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.fullcontact.com/\ndescription: >-\n  FullContact runs a Vanta-hosted Trust Center at trust.fullcontact.com. The\n  page returns 200 but is a client-side rendered single-page app, so its\n  certification list is not machine-readable from the served HTML. The one\n  certification FullContact names in plain text in its own documentation is\n  SOC 2, and that is the only one recorded here.\nurl: https://trust.fullcontact.com/\nplatform: Vanta\n\ncertifications:\n  - SOC 2\n\ncertifications_note: >-\n  SOC 2 is recorded on the strength of FullContact's own documentation, not on\n  the Trust Center HTML. No ISO 27001, PCI DSS, HIPAA or FedRAMP claim was\n  found in any machine-readable source; their absence here means \"not\n  observed\", not \"not held\" — the Trust Center may list more behind its\n  JavaScript.\n\nprivacy_program:\n  page: https://www.fullcontact.com/security/\n  claims:\n    - CCPA subject\
  \ access and deletion requests\n    - GDPR subject access and deletion requests\n    - '\"Do Not Sell My Personal Information\" handling'\n    - Contact data stored using 256-bit AES encryption at rest\n    - TLS configured with industry best practices\n\nevidence:\n  - source: https://trust.fullcontact.com/\n    status: 200\n    keywords: [trust center]\n    note: Vanta trust-report SPA; content loads from assets.vanta.com at runtime.\n  - source: https://docs.fullcontact.com/docs/authentication\n    status: 200\n    quote: '\"SOC 2. The hosted MCP Server runs inside FullContact''s existing SOC 2 boundary.\"'\n  - source: https://www.fullcontact.com/security/\n    status: 200\n    keywords: [GDPR, CCPA, encryption at rest, TLS]\n\nx-evidence:\n  fetched: '2026-08-14'\n  url: https://trust.fullcontact.com/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullcontact/refs/heads/main/security/fullcontact-trust-center.yml
summary_line: SOC 2
tags:
- Identity Resolution
- Customer Data
- Data Enrichment
- Person API
- Company API
- Privacy-Safe Identity
- Customer Recognition
trust_url: https://trust.fullcontact.com/
---
