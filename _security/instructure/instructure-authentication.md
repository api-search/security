---
api_key_in: []
api_specs:
- filename: instructure-externaltool-api-openapi.yml
  format: yaml
  label: Instructure ExternalTool API
  slug: instructure-externaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-externaltool-api-openapi.yml
- filename: instructure-lti-accountexternaltool-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountExternalTool API
  slug: instructure-lti-accountexternaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountexternaltool-api-openapi.yml
- filename: instructure-lti-accountlookup-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountLookup API
  slug: instructure-lti-accountlookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountlookup-api-openapi.yml
- filename: instructure-lti-dataservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::DataService API
  slug: instructure-lti-dataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-dataservice-api-openapi.yml
- filename: instructure-lti-ims-authentication-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Authentication API
  slug: instructure-lti-ims-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-authentication-api-openapi.yml
- filename: instructure-lti-ims-dynamicregistration-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::DynamicRegistration API
  slug: instructure-lti-ims-dynamicregistration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-dynamicregistration-api-openapi.yml
- filename: instructure-lti-ims-lineitem-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::LineItem API
  slug: instructure-lti-ims-lineitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-lineitem-api-openapi.yml
- filename: instructure-lti-ims-namesandrole-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::NamesAndRole API
  slug: instructure-lti-ims-namesandrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-namesandrole-api-openapi.yml
- filename: instructure-lti-ims-result-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Result API
  slug: instructure-lti-ims-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-result-api-openapi.yml
- filename: instructure-lti-membershipservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::MembershipService API
  slug: instructure-lti-membershipservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-membershipservice-api-openapi.yml
- filename: instructure-lti-toolconfigurationsapi-api-openapi.yml
  format: yaml
  label: Instructure Lti::ToolConfigurationsApi API
  slug: instructure-lti-toolconfigurationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-toolconfigurationsapi-api-openapi.yml
- filename: instructure-security-api-openapi.yml
  format: yaml
  label: Instructure Security API
  slug: instructure-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-security-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Instructure Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instructure secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instructure
provider_slug: instructure
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://{canvas_domain}/login/oauth2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{canvas_domain}/login/oauth2/token
  name: oauth2
  sources:
  - openapi/instructure-canvas-lti-openapi.yml
  type: oauth2
- description: Bearer token (access token)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/instructure-canvas-lti-openapi.yml
  type: http
slug: instructure-authentication
source_filename: instructure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instructure-canvas-lti-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{canvas_domain}/login/oauth2/auth\n    tokenUrl: https://{canvas_domain}/login/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/instructure-canvas-lti-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token (access token)\n  sources:\n  - openapi/instructure-canvas-lti-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/authentication/instructure-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
---
