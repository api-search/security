---
api_specs:
- filename: first-street-enterprise-api-openapi.yml
  format: yaml
  label: First Street Enterprise API
  slug: first-street-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-enterprise-api-openapi.yml
- filename: first-street-graphql-api-openapi.yml
  format: yaml
  label: First Street Graphql API
  slug: first-street-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-graphql-api-openapi.yml
- filename: first-street-maps-api-openapi.yml
  format: yaml
  label: First Street Maps API
  slug: first-street-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/openapi/first-street-maps-api-openapi.yml
certification_count: 1
certifications:
- SOC 2 Type II
description: First Street runs a Vanta-hosted trust center at security.firststreet.org (page title "First Street Trust Center"), linked from its own API repository README as the canonical place to read its security posture. The marketing security page at firststreet.org/security carries the SOC 2 Type II claim in its own title.
kind: trust-center
layout: security
name: First Street Trust Center
name_suffix: Trust Center
overview: First Street maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: First Street
provider_slug: first-street
slug: first-street-trust-center
source_filename: first-street-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nprobe: true\nsource: https://security.firststreet.org/\nurl: https://security.firststreet.org/\nplatform: Vanta\ndescription: >-\n  First Street runs a Vanta-hosted trust center at security.firststreet.org (page title\n  \"First Street Trust Center\"), linked from its own API repository README as the canonical\n  place to read its security posture. The marketing security page at\n  firststreet.org/security carries the SOC 2 Type II claim in its own title.\ncertifications:\n  - {name: SOC 2 Type II, evidence: 'https://firststreet.org/security — page title \"Security at First Street - SOC2 Type II Compliant\"; body references a SOC 2 Type II audit and penetration testing'}\nreadable_by_machine: false\nreadable_note: >-\n  The trust center is a client-rendered Vanta SPA — 5,442 bytes of shell HTML, with the\n  certification list, policies and subprocessors loaded by script and document downloads\n  behind a request form. Nothing on it\
  \ is machine-readable, and it answers 200 with the\n  same shell for every path (including a negative control), so it must not be treated as a\n  well-known surface.\ndata_handling:\n  uploaded_assets: >-\n    Enterprise portfolio uploads are encrypted at rest and the uploaded file is\n    \"automatically deleted after 7 days\".\n  access_scope: >-\n    Assets uploaded to projects are accessible by users within your Organization and your\n    Account Executive.\n  source: https://docs.firststreet.org/api/enterprise-api/workflow/upload-assets\nevidence:\n  - {source: 'https://security.firststreet.org/', http_status: 200, keywords: [trust, security, compliance, 'First Street Trust Center']}\n  - {source: 'https://firststreet.org/security', http_status: 200, keywords: ['soc 2', 'soc2 type ii', 'penetration test']}\n  - {source: 'https://github.com/FirstStreet/api/blob/HEAD/README.md', quote: 'For more information of our security policies, please visit our trust center'}\nmaintainers:\n  -\
  \ FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-street/refs/heads/main/security/first-street-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Climate
- Risk
- Environment
- Modeling
- Geospatial
- Insurance
- Real Estate
- Data
- GraphQL
- Mapping
trust_url: https://security.firststreet.org/
---
