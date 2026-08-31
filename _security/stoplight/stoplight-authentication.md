---
api_key_in: []
api_specs:
- filename: stoplight-versions-api-openapi.yml
  format: yaml
  label: Stoplight Versions API
  slug: stoplight-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/openapi/stoplight-versions-api-openapi.yml
auth_types: []
description: Authentication profile for the Stoplight surfaces. Stoplight publishes no consolidated API authentication reference; the two credential models below are the ones it actually documents.
kind: authentication
layout: security
method: searched
name: Stoplight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stoplight declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Stoplight
provider_slug: stoplight
scheme_count: 2
schemes:
- applies_to: Stoplight v1 (Classic) Platform API
  id: Authorization
  in: header
  method: derived
  name: Authorization
  note: Declared in components.securitySchemes of the v1 contract. The spec declares NO top-level `security` and no per-operation `security`, so the scheme is defined but never applied — an agent cannot tell from the contract which operations require it. Every operation does declare a 401 response, which is the only evidence that the header is required.
  source: openapi/stoplight-platform-v1-openapi.yml
  type: apiKey
- applies_to: Stoplight CLI (@stoplight/cli) project publishing
  id: project-token
  in: cli-flag
  method: searched
  name: --ci-token
  note: A per-project CI token, issued from https://{workspace}.stoplight.io/settings/{project}/automation and passed as `npx @stoplight/cli@5 push --ci-token {project-token} --url https://{workspace-name}.stoplight.io`. Scoped to one project, not to the workspace.
  source: https://docs.stoplight.io/docs/platform/f76c84240244f-publish-with-the-stoplight-cli
  type: apiKey
slug: stoplight-authentication
source_filename: stoplight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  openapi/stoplight-platform-v1-openapi.yml components.securitySchemes, plus\n  https://docs.stoplight.io/docs/platform/f76c84240244f-publish-with-the-stoplight-cli\ndocs: https://docs.stoplight.io/docs/platform/f76c84240244f-publish-with-the-stoplight-cli\nprovider: Stoplight\nproviderId: stoplight\ndescription: >-\n  Authentication profile for the Stoplight surfaces. Stoplight publishes no\n  consolidated API authentication reference; the two credential models below are\n  the ones it actually documents.\nschemes:\n  - id: Authorization\n    type: apiKey\n    in: header\n    name: Authorization\n    applies_to: Stoplight v1 (Classic) Platform API\n    source: openapi/stoplight-platform-v1-openapi.yml\n    method: derived\n    note: >-\n      Declared in components.securitySchemes of the v1 contract. The spec declares\n      NO top-level `security` and no per-operation `security`, so the scheme is\n      defined but never\
  \ applied — an agent cannot tell from the contract which\n      operations require it. Every operation does declare a 401 response, which is\n      the only evidence that the header is required.\n  - id: project-token\n    type: apiKey\n    in: cli-flag\n    name: --ci-token\n    applies_to: Stoplight CLI (@stoplight/cli) project publishing\n    source: https://docs.stoplight.io/docs/platform/f76c84240244f-publish-with-the-stoplight-cli\n    method: searched\n    note: >-\n      A per-project CI token, issued from\n      https://{workspace}.stoplight.io/settings/{project}/automation and passed as\n      `npx @stoplight/cli@5 push --ci-token {project-token} --url https://{workspace-name}.stoplight.io`.\n      Scoped to one project, not to the workspace.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nworkspace_sso:\n  supported: true\n  mechanisms:\n    - SAML SSO\n    - LDAP\n  docs: https://docs.stoplight.io/docs/platform/692808d0afabb-single-sign-on\n  note: >-\n    Human workspace\
  \ sign-in only (Azure, Google, Okta, OneLogin, Ping, Keycloak,\n    CyberArk setup guides are published). Not an API credential path.\ngaps:\n  - No published token-lifetime, rotation or revocation policy.\n  - No OAuth 2.0 or OpenID Connect surface for API access.\n  - securitySchemes is declared but never applied to any operation in the contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stoplight/refs/heads/main/authentication/stoplight-authentication.yml
summary_line: 2 schemes
tags:
- API Design
- API Documentation
- API Governance
- AsyncAPI
- Design-First
- Linting
- Mock Servers
- OpenAPI
- SmartBear API Hub
- Style Guides
---
