---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: backstage-events-backend-openapi.yaml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-events-backend-openapi.yaml
- filename: backstage-actions-api-openapi.yml
  format: yaml
  label: Backstage Actions API
  slug: backstage-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-actions-api-openapi.yml
- filename: backstage-auth-backend-openapi.yaml
  format: yaml
  label: Backstage Authentication API
  slug: backstage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-auth-backend-openapi.yaml
- filename: backstage-authorization-api-openapi.yml
  format: yaml
  label: Backstage Authorization API
  slug: backstage-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authorization-api-openapi.yml
- filename: backstage-documentation-api-openapi.yml
  format: yaml
  label: Backstage Documentation API
  slug: backstage-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-documentation-api-openapi.yml
- filename: backstage-catalog-backend-openapi.yaml
  format: yaml
  label: Backstage Entities API
  slug: backstage-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-catalog-backend-openapi.yaml
- filename: backstage-locations-api-openapi.yml
  format: yaml
  label: Backstage Locations API
  slug: backstage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-locations-api-openapi.yml
- filename: backstage-metadata-api-openapi.yml
  format: yaml
  label: Backstage Metadata API
  slug: backstage-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-metadata-api-openapi.yml
- filename: backstage-search-backend-openapi.yaml
  format: yaml
  label: Backstage Search API
  slug: backstage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-backend-openapi.yaml
- filename: backstage-sync-api-openapi.yml
  format: yaml
  label: Backstage Sync API
  slug: backstage-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-sync-api-openapi.yml
- filename: backstage-scaffolder-backend-openapi.yaml
  format: yaml
  label: Backstage Tasks API
  slug: backstage-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-scaffolder-backend-openapi.yaml
- filename: backstage-templates-api-openapi.yml
  format: yaml
  label: Backstage Templates API
  slug: backstage-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-templates-api-openapi.yml
- filename: backstage-token-verification-api-openapi.yml
  format: yaml
  label: Backstage Token Verification API
  slug: backstage-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-token-verification-api-openapi.yml
- filename: backstage-notifications-backend-openapi.yaml
  format: yaml
  label: Backstage Notifications API
  slug: backstage-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-notifications-backend-openapi.yaml
- filename: backstage-dynamic-features-openapi.yaml
  format: yaml
  label: Backstage Dynamic Feature Service API
  slug: backstage-dynamic-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-dynamic-features-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Backstage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backstage secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Backstage
provider_slug: backstage
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: backstage-auth
  sources:
  - openapi/backstage-actions-api-openapi.yml
  - openapi/backstage-authentication-api-openapi.yml
  - openapi/backstage-authorization-api-openapi.yml
  - openapi/backstage-documentation-api-openapi.yml
  - openapi/backstage-entities-api-openapi.yml
  - openapi/backstage-locations-api-openapi.yml
  - openapi/backstage-metadata-api-openapi.yml
  - openapi/backstage-search-api-openapi.yml
  - openapi/backstage-sync-api-openapi.yml
  - openapi/backstage-tasks-api-openapi.yml
  - openapi/backstage-templates-api-openapi.yml
  - openapi/backstage-token-verification-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/backstage-actions-api-openapi.yml
  - openapi/backstage-authentication-api-openapi.yml
  - openapi/backstage-authorization-api-openapi.yml
  - openapi/backstage-catalog-backend-openapi.yaml
  - openapi/backstage-documentation-api-openapi.yml
  - openapi/backstage-dynamic-features-openapi.yaml
  - openapi/backstage-entities-api-openapi.yml
  - openapi/backstage-events-backend-openapi.yaml
  - openapi/backstage-locations-api-openapi.yml
  - openapi/backstage-metadata-api-openapi.yml
  - openapi/backstage-notifications-backend-openapi.yaml
  - openapi/backstage-scaffolder-backend-openapi.yaml
  - openapi/backstage-search-api-openapi.yml
  - openapi/backstage-search-backend-openapi.yaml
  - openapi/backstage-sync-api-openapi.yml
  - openapi/backstage-tasks-api-openapi.yml
  - openapi/backstage-templates-api-openapi.yml
  - openapi/backstage-token-verification-api-openapi.yml
  type: http
slug: backstage-authentication
source_filename: backstage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/backstage-actions-api-openapi.yml, openapi/backstage-authentication-api-openapi.yml,\n  openapi/backstage-authorization-api-openapi.yml, openapi/backstage-catalog-backend-openapi.yaml,\n  openapi/backstage-documentation-api-openapi.yml, openapi/backstage-dynamic-features-openapi.yaml,\n  openapi/backstage-entities-api-openapi.yml, openapi/backstage-events-backend-openapi.yaml,\n  openapi/backstage-locations-api-openapi.yml, openapi/backstage-metadata-api-openapi.yml, openapi/backstage-notifications-backend-openapi.yaml,\n  openapi/backstage-scaffolder-backend-openapi.yaml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: backstage-auth\n  sources:\n  - openapi/backstage-actions-api-openapi.yml\n  - openapi/backstage-authentication-api-openapi.yml\n  - openapi/backstage-authorization-api-openapi.yml\n  - openapi/backstage-documentation-api-openapi.yml\n\
  \  - openapi/backstage-entities-api-openapi.yml\n  - openapi/backstage-locations-api-openapi.yml\n  - openapi/backstage-metadata-api-openapi.yml\n  - openapi/backstage-search-api-openapi.yml\n  - openapi/backstage-sync-api-openapi.yml\n  - openapi/backstage-tasks-api-openapi.yml\n  - openapi/backstage-templates-api-openapi.yml\n  - openapi/backstage-token-verification-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/backstage-actions-api-openapi.yml\n  - openapi/backstage-authentication-api-openapi.yml\n  - openapi/backstage-authorization-api-openapi.yml\n  - openapi/backstage-catalog-backend-openapi.yaml\n  - openapi/backstage-documentation-api-openapi.yml\n  - openapi/backstage-dynamic-features-openapi.yaml\n  - openapi/backstage-entities-api-openapi.yml\n  - openapi/backstage-events-backend-openapi.yaml\n  - openapi/backstage-locations-api-openapi.yml\n  - openapi/backstage-metadata-api-openapi.yml\n  - openapi/backstage-notifications-backend-openapi.yaml\n\
  \  - openapi/backstage-scaffolder-backend-openapi.yaml\n  - openapi/backstage-search-api-openapi.yml\n  - openapi/backstage-search-backend-openapi.yaml\n  - openapi/backstage-sync-api-openapi.yml\n  - openapi/backstage-tasks-api-openapi.yml\n  - openapi/backstage-templates-api-openapi.yml\n  - openapi/backstage-token-verification-api-openapi.yml\n\ndocs:\n  - https://backstage.io/docs/auth/\n  - https://backstage.io/docs/auth/identity-resolver\n  - https://backstage.io/docs/ai/mcp-actions\nsearched_enrichment:\n  note: >-\n    Upgraded from derived to searched on 2026-09-04 by reading the Backstage auth documentation and\n    the live OAuth discovery documents served by the project's demo deployment. Backstage is\n    self-hosted, so the concrete identity provider is the operator's choice; what Backstage itself\n    ships is the token model below.\n  models:\n    - name: Backstage user token (bearer JWT)\n      detail: >-\n        The frontend obtains a Backstage token from the auth backend\
  \ and sends it as\n        Authorization: Bearer <token> to plugin backends. This is the `JWT` bearer securityScheme\n        declared in every first-party plugin OpenAPI.\n    - name: Backstage service-to-service token\n      detail: >-\n        Plugin backends authenticate to each other with issued service tokens; the same bearer\n        header carries them.\n    - name: Cookie auth\n      detail: >-\n        A `backstage-auth` cookie is used for static asset / TechDocs style requests.\n    - name: External OAuth (MCP clients)\n      detail: >-\n        The MCP Actions endpoint is an OAuth 2.1-style protected resource. Observed live on\n        demo.backstage.io: RFC 9728 protected resource metadata pointing at an RFC 8414\n        authorization server with authorization_code + PKCE (S256), dynamic client registration,\n        token revocation, and Client ID Metadata Document (CIMD) support.\n  identity_providers_supported:\n    note: Backstage ships auth provider modules; the operator\
  \ picks one or more.\n    examples: [github, gitlab, google, okta, microsoft, auth0, oidc, atlassian, bitbucket, onelogin, saml/oauth2-proxy]\n  discovery_documents:\n    - well-known/backstage-demo-oauth-authorization-server.json\n    - well-known/backstage-demo-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/authentication/backstage-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open-Source
- Platform Engineering
- Software Templates
- CNCF
---
