---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-workspace-allowlisteddomains-api-openapi.yml
  format: yaml
  label: Google Workspace Allowlisted Domains API
  slug: google-workspace-allowlisteddomains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-allowlisteddomains-api-openapi.yml
- filename: google-workspace-customerlicense-api-openapi.yml
  format: yaml
  label: Google Workspace Customer License API
  slug: google-workspace-customerlicense-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-customerlicense-api-openapi.yml
- filename: google-workspace-customers-api-openapi.yml
  format: yaml
  label: Google Workspace Customers API
  slug: google-workspace-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-customers-api-openapi.yml
- filename: google-workspace-devices-api-openapi.yml
  format: yaml
  label: Google Workspace Devices API
  slug: google-workspace-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-devices-api-openapi.yml
- filename: google-workspace-groups-api-openapi.yml
  format: yaml
  label: Google Workspace Groups API
  slug: google-workspace-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-groups-api-openapi.yml
- filename: google-workspace-inboundoidcssoprofiles-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound Oidc SSO Profiles API
  slug: google-workspace-inboundoidcssoprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundoidcssoprofiles-api-openapi.yml
- filename: google-workspace-inboundsamlssoprofiles-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound Saml SSO Profiles API
  slug: google-workspace-inboundsamlssoprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundsamlssoprofiles-api-openapi.yml
- filename: google-workspace-inboundssoassignments-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound SSO Assignments API
  slug: google-workspace-inboundssoassignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundssoassignments-api-openapi.yml
- filename: google-workspace-operations-api-openapi.yml
  format: yaml
  label: Google Workspace Operations API
  slug: google-workspace-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-operations-api-openapi.yml
- filename: google-workspace-policies-api-openapi.yml
  format: yaml
  label: Google Workspace Policies API
  slug: google-workspace-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-policies-api-openapi.yml
- filename: google-workspace-subscriptions-api-openapi.yml
  format: yaml
  label: Google Workspace Subscriptions API
  slug: google-workspace-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-subscriptions-api-openapi.yml
- filename: google-workspace-userlicense-api-openapi.yml
  format: yaml
  label: Google Workspace User License API
  slug: google-workspace-userlicense-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-userlicense-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Google Workspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Workspace secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Workspace
provider_slug: google-workspace
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization for Google Workspace Admin operations.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/admin-sdk-directory-api.yml
  type: oauth2
slug: google-workspace-authentication
source_filename: google-workspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\ndocs: https://developers.google.com/workspace/guides/auth-overview\ndocs_note: \"Docs (HTTP 200, 2026-11-12) state: For accessing user data, you'll typically utilize OAuth 2.0 Client IDs or service accounts with domain-wide delegation of authority.\"\nsource: openapi/admin-sdk-directory-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 6\n  description: OAuth 2.0 authorization for Google Workspace Admin operations.\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n"
source_yaml_url: https://artifacts.apis.io/google-workspace/authentication/google-workspace-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
- Google Workspace
---
