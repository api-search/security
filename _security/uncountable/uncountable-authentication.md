---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Uncountable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uncountable declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Uncountable
provider_slug: uncountable
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization code with PKCE, recommended by Uncountable for integrations and third-party tools. Advertised by the discovery document on both the US and EU application hosts.
  flows:
    authorization_code:
      authorization_url: https://app.uncountable.com/oauth2/authorize
      pkce_methods:
      - S256
      refresh_supported: true
      scopes:
        CAD: CAD-related access
        EXTERNAL_API_READ: read access to the External API
        EXTERNAL_API_WRITE: write access to the External API
      token_url: https://app.uncountable.com/oauth2/token
  id_token_signing_alg:
  - RS256
  issuer: https://app.uncountable.com
  jwks_uri: https://app.uncountable.com/.well-known/jwks.json
  key: oauth2
  preferred: true
  token_endpoint_auth_methods:
  - none
  type: oauth2
- description: Basic authentication, documented for "simpler or legacy use cases". Requests may be made as a personal API key tied to an individual user account, or as a robot user (service account) for integrations and automated tasks.
  key: basic
  preferred: false
  scheme: basic
  source: https://www.support.uncountable.com/knowledge-base/api-access-and-permissions-in-uncountable/
  type: http
slug: uncountable-authentication
source_filename: uncountable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://app.uncountable.com/.well-known/openid-configuration (HTTP 200) +\n  https://www.support.uncountable.com/knowledge-base/api-access-and-permissions-in-uncountable/\ndocs: https://www.support.uncountable.com/knowledge-base/api-access-and-permissions-in-uncountable/\nnote: >-\n  Uncountable publishes no public OpenAPI, so this profile is not derived from\n  securitySchemes. It is read from the live OAuth 2.0 / OpenID Connect discovery\n  document served anonymously at each application host, plus the public knowledgebase\n  article on API access and permissions.\nschemes:\n- key: oauth2\n  type: oauth2\n  preferred: true\n  description: >-\n    OAuth 2.0 authorization code with PKCE, recommended by Uncountable for integrations\n    and third-party tools. Advertised by the discovery document on both the US and EU\n    application hosts.\n  flows:\n    authorization_code:\n      authorization_url: https://app.uncountable.com/oauth2/authorize\n\
  \      token_url: https://app.uncountable.com/oauth2/token\n      refresh_supported: true\n      pkce_methods:\n      - S256\n      scopes:\n        EXTERNAL_API_READ: read access to the External API\n        EXTERNAL_API_WRITE: write access to the External API\n        CAD: CAD-related access\n  token_endpoint_auth_methods:\n  - none\n  id_token_signing_alg:\n  - RS256\n  jwks_uri: https://app.uncountable.com/.well-known/jwks.json\n  issuer: https://app.uncountable.com\n- key: basic\n  type: http\n  scheme: basic\n  preferred: false\n  description: >-\n    Basic authentication, documented for \"simpler or legacy use cases\". Requests may be\n    made as a personal API key tied to an individual user account, or as a robot user\n    (service account) for integrations and automated tasks.\n  source: https://www.support.uncountable.com/knowledge-base/api-access-and-permissions-in-uncountable/\nregions:\n- region: us\n  issuer: https://app.uncountable.com\n  discovery: https://app.uncountable.com/.well-known/openid-configuration\n\
  \  http_status: 200\n- region: eu\n  issuer: https://appeu.uncountable.com\n  discovery: https://appeu.uncountable.com/.well-known/openid-configuration\n  http_status: 200\nclient_registration:\n  dynamic: false\n  dynamic_probe:\n    url: https://app.uncountable.com/oauth2/register\n    method: POST\n    http_status: 302\n    note: redirects to /signin — RFC 7591 dynamic client registration is not offered anonymously\n  manual: >-\n    An administrator creates the OAuth client in Uncountable under\n    User Administration -> OAuth. Clients are scoped to a single schema/account.\n  client_id_metadata_document_supported: true\nauthorization_model:\n  model: rbac\n  description: >-\n    Role-based access control is enforced identically across the web UI and the API, at\n    project, experiment and dataset level. API responses are filtered server-side to the\n    caller's permissions, so no client-side filtering is required.\n  unauthorized_status: 403\n  audit_logged: true\nsso:\n  saml2:\
  \ true\n  scim: true\n  mfa: true\n  ip_allowlisting: true\n  source: https://www.uncountable.com/uncountable-security\n  note: >-\n    SAML v2 SSO, SCIM automated provisioning, MFA and IP allowlisting are stated on the\n    company security page. These govern platform/user sign-in, not the External API\n    token flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncountable/refs/heads/main/authentication/uncountable-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Laboratory Informatics
- LIMS
- Electronic Lab Notebook
- R&D Data Management
- Product Lifecycle Management
- Quality Management
- Materials Science
- Chemicals
- Artificial Intelligence
- Model Context Protocol
---
