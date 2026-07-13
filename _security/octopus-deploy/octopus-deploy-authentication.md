---
api_key_in:
- header
api_specs:
- filename: octopus-deploy-openapi.yml
  format: yaml
  label: Octopus Deploy REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/openapi/octopus-deploy-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Octopus Deploy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Octopus Deploy secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Octopus Deploy
provider_slug: octopus-deploy
scheme_count: 2
schemes:
- description: 'Preferred authentication mechanism. Generate an API key from

    your Octopus user profile. The key may also be supplied as the

    `apikey` query parameter for simple cases.'
  in: header
  name: ApiKeyAuth
  parameter: X-Octopus-ApiKey
  sources:
  - openapi/octopus-deploy-openapi.yml
  type: apiKey
- description: 'Authenticate by exchanging an OpenID Connect identity token from

    a trusted external system (for example GitHub Actions) for a

    short-lived Octopus access token.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://your-octopus-instance/api/oidc/token
  name: OidcAuth
  sources:
  - openapi/octopus-deploy-openapi.yml
  type: oauth2
slug: octopus-deploy-authentication
source_filename: octopus-deploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/octopus-deploy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Octopus-ApiKey\n  description: |-\n    Preferred authentication mechanism. Generate an API key from\n    your Octopus user profile. The key may also be supplied as the\n    `apikey` query parameter for simple cases.\n  sources:\n  - openapi/octopus-deploy-openapi.yml\n- name: OidcAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-octopus-instance/api/oidc/token\n    scopes: 0\n  description: |-\n    Authenticate by exchanging an OpenID Connect identity token from\n    a trusted external system (for example GitHub Actions) for a\n    short-lived Octopus access token.\n  sources:\n  - openapi/octopus-deploy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopus-deploy/refs/heads/main/authentication/octopus-deploy-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- DevOps
- Continuous Delivery
- Deployment Automation
- Release Management
- Runbooks
- CI/CD
---
