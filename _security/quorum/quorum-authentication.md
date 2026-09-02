---
api_key_in: []
api_specs:
- filename: quorum-divisionorders-api-openapi.yml
  format: yaml
  label: Quorum Software DivisionOrders API
  slug: quorum-divisionorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-divisionorders-api-openapi.yml
- filename: quorum-leases-api-openapi.yml
  format: yaml
  label: Quorum Software Leases API
  slug: quorum-leases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-leases-api-openapi.yml
- filename: quorum-owners-api-openapi.yml
  format: yaml
  label: Quorum Software Owners API
  slug: quorum-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-owners-api-openapi.yml
- filename: quorum-tracts-api-openapi.yml
  format: yaml
  label: Quorum Software Tracts API
  slug: quorum-tracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-tracts-api-openapi.yml
- filename: quorum-wells-api-openapi.yml
  format: yaml
  label: Quorum Software Wells API
  slug: quorum-wells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/openapi/quorum-wells-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Quorum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Quorum Software secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Quorum Software
provider_slug: quorum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.quorumsoftware.com/oauth2/token
  name: oauth2
  sources:
  - openapi/quorum-land-management-openapi.yml
  type: oauth2
slug: quorum-authentication
source_filename: quorum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quorum-land-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.quorumsoftware.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/quorum-land-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/authentication/quorum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Oil and Gas
- Upstream
- Land Management
- Royalty Accounting
- Production Reporting
---
