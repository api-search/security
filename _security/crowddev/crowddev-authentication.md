---
api_key_in: []
api_specs:
- filename: crowddev-advisories-api-openapi.yml
  format: yaml
  label: Crowd.dev Advisories API
  slug: crowddev-advisories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-advisories-api-openapi.yml
- filename: crowddev-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Affiliations API
  slug: crowddev-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-affiliations-api-openapi.yml
- filename: crowddev-contacts-api-openapi.yml
  format: yaml
  label: Crowd.dev Contacts API
  slug: crowddev-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-contacts-api-openapi.yml
- filename: crowddev-dashboard-api-openapi.yml
  format: yaml
  label: Crowd.dev Dashboard API
  slug: crowddev-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-dashboard-api-openapi.yml
- filename: crowddev-maintainer-roles-api-openapi.yml
  format: yaml
  label: Crowd.dev Maintainer Roles API
  slug: crowddev-maintainer-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-maintainer-roles-api-openapi.yml
- filename: crowddev-member-affiliations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Affiliations API API
  slug: crowddev-member-affiliations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-affiliations-api-api-openapi.yml
- filename: crowddev-member-identities-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Identities API
  slug: crowddev-member-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-identities-api-openapi.yml
- filename: crowddev-member-organizations-api-api-openapi.yml
  format: yaml
  label: Crowd.dev Member Organizations API API
  slug: crowddev-member-organizations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-member-organizations-api-api-openapi.yml
- filename: crowddev-members-api-openapi.yml
  format: yaml
  label: Crowd.dev Members API
  slug: crowddev-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-members-api-openapi.yml
- filename: crowddev-organizations-api-openapi.yml
  format: yaml
  label: Crowd.dev Organizations API
  slug: crowddev-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-organizations-api-openapi.yml
- filename: crowddev-packages-api-openapi.yml
  format: yaml
  label: Crowd.dev Packages API
  slug: crowddev-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-packages-api-openapi.yml
- filename: crowddev-project-affiliations-api-openapi.yml
  format: yaml
  label: Crowd.dev Project Affiliations API
  slug: crowddev-project-affiliations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-project-affiliations-api-openapi.yml
- filename: crowddev-stewardship-actions-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship Actions API
  slug: crowddev-stewardship-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-actions-api-openapi.yml
- filename: crowddev-stewardship-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardship API
  slug: crowddev-stewardship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardship-api-openapi.yml
- filename: crowddev-stewardships-api-openapi.yml
  format: yaml
  label: Crowd.dev Stewardships API
  slug: crowddev-stewardships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-stewardships-api-openapi.yml
- filename: crowddev-work-experiences-api-openapi.yml
  format: yaml
  label: Crowd.dev Work Experiences API
  slug: crowddev-work-experiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-work-experiences-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crowddev Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Crowd.dev secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Crowd.dev
provider_slug: crowddev
scheme_count: 4
schemes:
- description: OAuth 2.0 client credentials flow via Auth0. Used by LFX One for member, organization and affiliation management endpoints.
  flows:
  - flow: clientCredentials
    scopes: 12
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: OAuth2Bearer
  sources:
  - openapi/crowddev-cdp-public-openapi.yml
  type: oauth2
- description: Auth0 machine-to-machine client-credentials flow for the Akrites external consumer. Modeled as oauth2/clientCredentials rather than http/bearer because OpenAPI only permits non-empty scope arrays on oauth2 / openIdConnect schemes.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: M2MBearer
  sources:
  - openapi/crowddev-cdp-akrites-external-openapi.yml
  type: oauth2
- description: Static API key presented as an HTTP bearer token, with scopes managed in the CDP database rather than in Auth0. Declared on the Affiliations endpoints.
  name: StaticApiKey
  scheme: bearer
  sources:
  - openapi/crowddev-cdp-public-openapi.yml
  type: http
- bearerFormat: JWT
  description: Auth0 M2M or user-session JWT presented as a bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crowddev-cdp-akrites-openapi.yml
  - openapi/crowddev-cdp-ossprey-openapi.yml
  - openapi/crowddev-cdp-packages-openapi.yml
  - openapi/crowddev-cdp-public-openapi.yml
  - openapi/crowddev-cdp-stewardships-openapi.yml
  - openapi/crowddev-cm-id-openapi.yml
  type: http
slug: crowddev-authentication
source_filename: crowddev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\ndocs:\n- https://github.com/linuxfoundation/crowd.dev/blob/main/docs/adr/0016-akrites-cdp-public-api-authentication.md\n- https://github.com/linuxfoundation/crowd.dev/tree/main/backend/src/api/public\nderived_from:\n- openapi/crowddev-cdp-akrites-external-openapi.yml\n- openapi/crowddev-cdp-akrites-openapi.yml\n- openapi/crowddev-cdp-ossprey-openapi.yml\n- openapi/crowddev-cdp-packages-openapi.yml\n- openapi/crowddev-cdp-public-openapi.yml\n- openapi/crowddev-cdp-stewardships-openapi.yml\n- openapi/crowddev-cm-id-openapi.yml\nnote: >-\n  Upgraded from derived to searched on 2026-08-14 against ADR-0016 (proposed, 2026-07-22), the\n  first-party design record for CDP Public API authentication published in the Apache-2.0\n  monorepo. It supplies what the OpenAPI alone could not: the identity provider, the audience\n \
  \ values, the client authentication methods, the enforcement point, and how credentials are\n  actually delivered.\n\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  identity_provider: Auth0 (Linux Foundation tenant)\n  issuer: https://linuxfoundation.auth0.com/\n  token_endpoint: https://linuxfoundation.auth0.com/oauth/token\n  discovery: well-known/crowddev-auth0-openid-configuration.json\n  self_serve_credentials: false\n\naudiences:\n- environment: production\n  audience: https://cm.lfx.dev/api/\n  source: ADR-0016\n- environment: staging-and-dev\n  audience: https://lf-staging.crowd.dev/api/\n  source: ADR-0016\n\nauth0_api: cdp_public_api\n\nclient_auth_methods:\n- method: client_secret_post\n  client: lfx_one\n  used_by: LFX One / Self Serve\n  source: ADR-0016\n- method: private_key_jwt\n  client: Akrites Enclave\n  used_by: Akrites (external consumer, hosted on GCP)\n  source: ADR-0016\n  note: >-\n    Akrites signs an RSA `client_assertion`\
  \ JWT and exchanges it at Auth0 for a short-lived bearer\n    token. CDP never sees the client_id or secret - it verifies only the Auth0-signed token, so\n    from CDP's side both client auth methods produce shape-identical tokens.\n\nenforcement:\n  middleware: oauth2Middleware (verifies exactly one audience) + per-endpoint requireScopes\n  client_allowlist: false\n  note: >-\n    ADR-0016 - \"CDP's per-endpoint `requireScopes` middleware is the sole enforcement point at the\n    API layer - no `azp` allowlist or other client-identity inspection in CDP source.\" Consumer\n    isolation is claim-based: Auth0 grants the Akrites-namespaced scopes only to the\n    `Akrites Enclave` client.\n\ncredential_delivery:\n  automated: false\n  owner: lfx-secrets-management\n  channel: 1Password vault item (RSA private key, client_id, credential kid)\n  rotation: coordinated manually between LF and the consumer\n  reason: >-\n    ADR-0016 - lfx-secrets-management delivers to AWS destinations and 1Password\
  \ only; the Akrites\n    service runs on GCP, which is not a supported destination. LF CloudOps has GCP support as a\n    backlog item.\n\nschemes:\n- name: OAuth2Bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n    scopes: 12\n  description: >-\n    OAuth 2.0 client credentials flow via Auth0. Used by LFX One for member, organization and\n    affiliation management endpoints.\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- name: M2MBearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n    scopes: 3\n  description: >-\n    Auth0 machine-to-machine client-credentials flow for the Akrites external consumer. Modeled as\n    oauth2/clientCredentials rather than http/bearer because OpenAPI only permits non-empty scope\n    arrays on oauth2 / openIdConnect schemes.\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n- name:\
  \ StaticApiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Static API key presented as an HTTP bearer token, with scopes managed in the CDP database\n    rather than in Auth0. Declared on the Affiliations endpoints.\n  sources:\n  - openapi/crowddev-cdp-public-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Auth0 M2M or user-session JWT presented as a bearer token.\n  sources:\n  - openapi/crowddev-cdp-akrites-openapi.yml\n  - openapi/crowddev-cdp-ossprey-openapi.yml\n  - openapi/crowddev-cdp-packages-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n  - openapi/crowddev-cdp-stewardships-openapi.yml\n  - openapi/crowddev-cm-id-openapi.yml\n\nrelated:\n  scopes: scopes/crowddev-scopes.yml\n  rate_limits: rate-limits/crowddev-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/authentication/crowddev-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open-Source
- Community Data Platform
- Open Source Intelligence
---
