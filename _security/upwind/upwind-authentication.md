---
api_key_in: []
api_specs:
- filename: upwind-access-management-api-openapi.yml
  format: yaml
  label: Upwind access-management API
  slug: upwind-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-access-management-api-openapi.yml
- filename: upwind-api-security-api-openapi.yml
  format: yaml
  label: Upwind api-security API
  slug: upwind-api-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-api-security-api-openapi.yml
- filename: upwind-cloud-accounts-api-openapi.yml
  format: yaml
  label: Upwind cloud-accounts API
  slug: upwind-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-cloud-accounts-api-openapi.yml
- filename: upwind-configurations-api-openapi.yml
  format: yaml
  label: Upwind configurations API
  slug: upwind-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-configurations-api-openapi.yml
- filename: upwind-events-api-openapi.yml
  format: yaml
  label: Upwind events API
  slug: upwind-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-events-api-openapi.yml
- filename: upwind-integrations-api-openapi.yml
  format: yaml
  label: Upwind integrations API
  slug: upwind-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-integrations-api-openapi.yml
- filename: upwind-inventory-api-openapi.yml
  format: yaml
  label: Upwind Inventory API
  slug: upwind-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-inventory-api-openapi.yml
- filename: upwind-packages-api-openapi.yml
  format: yaml
  label: Upwind packages API
  slug: upwind-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-packages-api-openapi.yml
- filename: upwind-shiftleft-api-openapi.yml
  format: yaml
  label: Upwind shiftleft API
  slug: upwind-shiftleft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-shiftleft-api-openapi.yml
- filename: upwind-threats-api-openapi.yml
  format: yaml
  label: Upwind threats API
  slug: upwind-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-threats-api-openapi.yml
- filename: upwind-vulnerabilities-api-openapi.yml
  format: yaml
  label: Upwind vulnerabilities API
  slug: upwind-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-vulnerabilities-api-openapi.yml
- filename: upwind-workflows-api-openapi.yml
  format: yaml
  label: Upwind workflows API
  slug: upwind-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-workflows-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Upwind Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Upwind secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Upwind
provider_slug: upwind
scheme_count: 1
schemes:
- description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token with an audience matching the regional API host (https://api.upwind.io, https://api.eu.upwind.io, or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.upwind.io/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/upwind-management-v1-openapi.yml
  - openapi/upwind-management-v2-openapi.yml
  type: oauth2
slug: upwind-authentication
source_filename: upwind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/upwind-management-v1-openapi.yml, openapi/upwind-management-v2-openapi.yml\ndocs: https://docs.upwind.io/restapi/v1/introduction\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.upwind.io/oauth/token\n    scopes: 0\n  description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind\n    Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token\n    with an audience matching the regional API host (https://api.upwind.io, https://api.eu.upwind.io,\n    or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'\n  sources:\n  - openapi/upwind-management-v1-openapi.yml\n  - openapi/upwind-management-v2-openapi.yml\ndetails:\n  issuer: https://auth.upwind.io/ (Auth0-hosted; OIDC discovery\
  \ at /.well-known/openid-configuration, see well-known/upwind-openid-configuration.json)\n  token_format: JWT (Bearer authentication scheme)\n  token_lifetime: All tokens automatically expire after 24 hours.\n  audience_required: true\n  audiences:\n    - https://api.upwind.io\n    - https://api.eu.upwind.io\n    - https://api.me.upwind.io\n  credential_types:\n    - {type: Cloud account, usage: 'Establish a connection with a cloud service provider (AWS, GCP, Azure, Oracle)'}\n    - {type: Sensor, usage: Deploy an Upwind Sensor using Helm or Bash}\n    - {type: API, usage: Use the Management REST API}\n    - {type: Integration, usage: 'Third-party integrations (Slack, Kubernetes Audit Logs, GitHub Actions, ...)'}\n  rbac: >-\n    API credentials carry a scope and roles bounded by the creating member's own access (no\n    privilege escalation); the scope of existing credentials is immutable — generate new\n    credentials to change resource boundaries. Default limit of 20 credentials per\
  \ organization.\n  credentials_docs: https://docs.upwind.io/settings/credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/authentication/upwind-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Security
- Cloud Security
- CNAPP
- Vulnerability Management
- Container Security
- Kubernetes
- API Security
- Threat Detection
- Data Security
---
