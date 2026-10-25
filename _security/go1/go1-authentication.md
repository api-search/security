---
anonymous_access: false
api_key_in: []
api_specs:
- filename: go1-categories-api-openapi.yml
  format: yaml
  label: Go1 Categories API
  slug: go1-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-categories-api-openapi.yml
- filename: go1-collections-api-openapi.yml
  format: yaml
  label: Go1 Collections API
  slug: go1-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-collections-api-openapi.yml
- filename: go1-compliance-api-openapi.yml
  format: yaml
  label: Go1 Compliance API
  slug: go1-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-compliance-api-openapi.yml
- filename: go1-enrollments-api-openapi.yml
  format: yaml
  label: Go1 Enrollments API
  slug: go1-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-enrollments-api-openapi.yml
- filename: go1-files-api-openapi.yml
  format: yaml
  label: Go1 Files API
  slug: go1-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-files-api-openapi.yml
- filename: go1-learning-objects-api-openapi.yml
  format: yaml
  label: Go1 Learning objects API
  slug: go1-learning-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-learning-objects-api-openapi.yml
- filename: go1-plans-api-openapi.yml
  format: yaml
  label: Go1 Plans API
  slug: go1-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-plans-api-openapi.yml
- filename: go1-play-links-api-openapi.yml
  format: yaml
  label: Go1 Play links API
  slug: go1-play-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-play-links-api-openapi.yml
- filename: go1-playlists-api-openapi.yml
  format: yaml
  label: Go1 Playlists API
  slug: go1-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-playlists-api-openapi.yml
- filename: go1-portals-api-openapi.yml
  format: yaml
  label: Go1 Portals API
  slug: go1-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-portals-api-openapi.yml
- filename: go1-restrictions-api-openapi.yml
  format: yaml
  label: Go1 Restrictions API
  slug: go1-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-restrictions-api-openapi.yml
- filename: go1-scim-api-openapi.yml
  format: yaml
  label: Go1 SCIM API
  slug: go1-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-scim-api-openapi.yml
- filename: go1-user-accounts-api-openapi.yml
  format: yaml
  label: Go1 User accounts API
  slug: go1-user-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-user-accounts-api-openapi.yml
- filename: go1-webhooks-api-openapi.yml
  format: yaml
  label: Go1 Webhooks API
  slug: go1-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Go1 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Go1 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Go1
provider_slug: go1
scheme_count: 1
schemes:
- description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations use the authorization_code flow. Access tokens are valid for 12 hours.
  flows:
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://auth.go1.com/oauth/token
  - authorizationUrl: https://auth.go1.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://auth.go1.com/oauth/token
  name: OAuth2
  sources:
  - openapi/go1-openapi.yml
  type: oauth2
slug: go1-authentication
source_filename: go1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://developers.go1.com/docs/developer-tools/auth/overview-auth/\ndocs: https://developers.go1.com/docs/developer-tools/auth/overview-auth/\nverified:\n- https://developers.go1.com/docs/developer-tools/auth/grant-client-credentials\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.go1.com/oauth/token\n    scopes: 8\n  - flow: authorizationCode\n    authorizationUrl: https://auth.go1.com/oauth/authorize\n    tokenUrl: https://auth.go1.com/oauth/token\n    scopes: 8\n  description: OAuth 2.0. Server-to-server integrations use the client_credentials flow; user-context integrations\n    use the authorization_code flow. Access tokens are valid for 12 hours.\n  sources:\n  - openapi/go1-openapi.yml\nscopes_docs: https://developers.go1.com/docs/developer-tools/auth/oauth-scopes/\n\
  note: 'Docs: \"Go1 uses OAuth 2.0, an industry-standard framework, for authentication.\" Credentials (client_id, client_secret)\n  come from a Go1 Developer App. Token endpoint taken from the OpenAPI securitySchemes; it was not called (GET/HEAD/OPTIONS-only\n  probe policy).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/authentication/go1-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- EdTech
- Learning
- E-Learning
- Corporate Training
- Content
- LMS
- Education
- Webhook
---
