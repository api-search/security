---
api_key_in: []
api_specs:
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profiles API
  slug: memberclicks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profile Search API
  slug: memberclicks-profile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Attributes API
  slug: memberclicks-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Member Types and Statuses API
  slug: memberclicks-member-types-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Groups API
  slug: memberclicks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Events API
  slug: memberclicks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Continuing Education API
  slug: memberclicks-continuing-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Memberclicks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: MemberClicks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: MemberClicks
provider_slug: memberclicks
scheme_count: 1
schemes:
- description: OAuth 2.0. Obtain a bearer token from /oauth/v1/token using HTTP Basic client credentials (Base64 clientId:clientSecret) with scope read, write, or read write.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://{orgId}.memberclicks.net/oauth/v1/token
  name: oauth2
  sources:
  - openapi/memberclicks-openapi.yml
  type: oauth2
slug: memberclicks-authentication
source_filename: memberclicks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/memberclicks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{orgId}.memberclicks.net/oauth/v1/token\n    scopes: 2\n  description: OAuth 2.0. Obtain a bearer token from /oauth/v1/token using HTTP Basic client\n    credentials (Base64 clientId:clientSecret) with scope read, write, or read write.\n  sources:\n  - openapi/memberclicks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/authentication/memberclicks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- CRM
- Personify
---
