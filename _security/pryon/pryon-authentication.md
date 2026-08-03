---
api_key_in:
- header
api_specs:
- filename: pryon-admin-openapi.json
  format: json
  label: Pryon Admin API
  slug: pryon-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-admin-openapi.json
- filename: pryon-retrieval-may2025-openapi.json
  format: json
  label: Pryon Retrieval API
  slug: pryon-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-retrieval-may2025-openapi.json
- filename: pryon-generative-openapi.json
  format: json
  label: Pryon Generative API
  slug: pryon-generative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-generative-openapi.json
- filename: pryon-knowledge-collections-may2025-openapi.json
  format: json
  label: Pryon Knowledge Collections API
  slug: pryon-knowledge-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-knowledge-collections-may2025-openapi.json
- filename: pryon-exchange-may2025-openapi.json
  format: json
  label: Pryon Exchange API
  slug: pryon-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-exchange-may2025-openapi.json
- filename: pryon-feedback-august2025-openapi.json
  format: json
  label: Pryon Feedback API
  slug: pryon-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-feedback-august2025-openapi.json
- filename: pryon-universal-connector-may2025-openapi.json
  format: json
  label: Pryon Universal Connector API
  slug: pryon-universal-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-universal-connector-may2025-openapi.json
- filename: pryon-user-defined-metadata-may2025-openapi.json
  format: json
  label: Pryon User-Defined Metadata API
  slug: pryon-user-defined-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-user-defined-metadata-may2025-openapi.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pryon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Pryon secures its APIs with oauth2 and apiKey across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Pryon
provider_slug: pryon
scheme_count: 1
schemes:
- description: The Pryon APIs are authenicated with an OAuth2 Bearer token.
  in: header
  name: oauth2_token
  note: 'Declared verbatim in the published spec, including the typo. The working header is "Authorization: Bearer <access_token>".'
  parameter: 'Authoriation: Bearer'
  sources:
  - openapi/pryon-retrieval-may2025-openapi.json
  type: apiKey
slug: pryon-authentication
source_filename: pryon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/ (22 harvested Pryon OpenAPI documents)\ndocs: https://docs.pryon.com/reference/api-authentication\nrecipes: https://docs.pryon.com/recipes/authenticating-to-the-pryon-apis\nsso_docs: https://docs.pryon.com/docs/single-sign-on\nscenarios_docs: https://docs.pryon.com/docs/authentication-scenarios\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  identity_provider: Keycloak 26.4 (per the Q1 2026 platform release notes); customer IdPs\n    federated via OIDC for SSO, with multi-tenancy across multiple IdPs on one email domain.\nmodel: |\n  Every Pryon API is authenticated with an OAuth 2.0 JSON Web Token bearer access token.\n  Server-to-server integrations use the client-credentials grant against the platform's OAuth\n  token endpoint; end-user applications obtain user tokens through an OpenID Connect implicit\n  or authorization-code flow federated to the tenant's identity\
  \ provider. Client credentials\n  are issued by the customer's Pryon Solutions Manager, or by the organization administrator\n  for on-premises deployments — there is no self-serve key issuance.\noauth2:\n  grant_type: client_credentials\n  audience: https://pryon/api\n  token_endpoints:\n  - {platform: classic, url: 'https://auth.pryon.net/oauth/token'}\n  - {platform: unified, url: 'https://auth-us-central-1.pryon.net/oauth/token'}\n  request:\n    method: POST\n    content_type: application/json\n    fields: [client_id, client_secret, audience, grant_type]\n  response:\n    fields: [access_token, token_type, expires_in]\n    token_type: Bearer\n    default_expires_in: 86400\n  reuse_guidance: Pryon documents retaining and reusing server tokens for their full lifetime\n    rather than requesting a new token per API call.\n  scopes: []\n  scopes_note: No OAuth scope surface is documented or declared in any published spec; a\n    client-credentials token is bounded by the service account\
  \ Pryon issues it to. No\n    scopes/ artifact is emitted for this provider.\n  discovery:\n    openid_configuration: null\n    note: The token hosts do not resolve from the public internet, so no RFC 8414 / OIDC\n      discovery document could be retrieved anonymously (see well-known/pryon-well-known.yml).\n  reference: https://tools.ietf.org/html/rfc6749\nschemes:\n- name: oauth2_token\n  type: apiKey\n  in: header\n  parameter: 'Authoriation: Bearer'\n  description: The Pryon APIs are authenicated with an OAuth2 Bearer token.\n  note: >-\n    Declared verbatim in the published spec, including the typo. The working header is\n    \"Authorization: Bearer <access_token>\".\n  sources:\n  - openapi/pryon-retrieval-may2025-openapi.json\nrequest_headers:\n- {name: Authorization, operations: 81, note: 'Bearer <access_token>'}\n- {name: Authentication, operations: 140, note: 'Alternate spelling declared across the harvested specs for the same credential.'}\n- {name: x-pryon-org-id, operations:\
  \ 34, note: 'Organization (tenant) identifier on multi-tenant administrative operations.'}\ngaps:\n- The published specs model an OAuth 2.0 bearer token as an apiKey header, understating the\n  flow the documentation describes. overlays/ adds a correct oauth2 clientCredentials\n  securityScheme without mutating the harvested spec.\n- Two different header names are declared for the same credential across the spec corpus.\n- No securityScheme is applied at the operation or document level in any spec, so the\n  contract does not machine-declare that these operations require authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/authentication/pryon-authentication.yml
summary_line: oauth2/apiKey · 1 scheme
tags:
- Artificial Intelligence
- Retrieval Augmented Generation
- Enterprise Search
- Knowledge Management
- Generative AI
- Document Ingestion
- Content Connectors
- Agents
- Machine Learning
- Company
---
