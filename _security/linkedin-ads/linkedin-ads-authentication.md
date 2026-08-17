---
api_key_in: []
api_specs:
- filename: linkedin-ads-adaccounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdAccounts API
  slug: linkedin-ads-adaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adaccounts-api-openapi.yml
- filename: linkedin-ads-adbudgetpricing-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdBudgetPricing API
  slug: linkedin-ads-adbudgetpricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adbudgetpricing-api-openapi.yml
- filename: linkedin-ads-adtargetingentities-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingEntities API
  slug: linkedin-ads-adtargetingentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingentities-api-openapi.yml
- filename: linkedin-ads-adtargetingfacets-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingFacets API
  slug: linkedin-ads-adtargetingfacets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingfacets-api-openapi.yml
- filename: linkedin-ads-audiencecounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AudienceCounts API
  slug: linkedin-ads-audiencecounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-audiencecounts-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Linkedin Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: LinkedIn Marketing API secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
scheme_count: 3
schemes:
- description: OAuth 2.0 three-legged (authorization code) flow — the flow every Marketing API call uses. The member consents to the full requested scope set; scopes cannot be selected individually, and changing an app's scopes forces members to re-authenticate.
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2
  sources:
  - openapi/linkedin-ads-openapi.yml
  type: oauth2
- description: Sign In with LinkedIn using OpenID Connect. Discovery document served live and captured verbatim in well-known/linkedin-ads-openid-configuration.json.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.linkedin.com/oauth
  jwks_uri: https://www.linkedin.com/oauth/openid/jwks
  name: OpenIDConnect
  openIdConnectUrl: https://www.linkedin.com/oauth/.well-known/openid-configuration
  scopes:
  - openid
  - profile
  - email
  sources:
  - well-known/linkedin-ads-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://api.linkedin.com/v2/userinfo
- description: Two-legged flow, available only to selected partner programs; it grants application-level access with no member context and is not used by the advertising surface.
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2ClientCredentials
  sources:
  - https://learn.microsoft.com/en-us/linkedin/shared/authentication/client-credentials-flow
  type: oauth2
slug: linkedin-ads-authentication
source_filename: linkedin-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/linkedin-ads-openapi.yml\ndocs: https://learn.microsoft.com/en-us/linkedin/shared/authentication/authorization-code-flow\nnote: >-\n  Derived from the repository OpenAPI, then upgraded from LinkedIn's own auth\n  documentation and a live fetch of the OpenID Connect discovery document at\n  https://www.linkedin.com/oauth/.well-known/openid-configuration (HTTP 200).\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n        tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n        scopes: 4\n    description: >-\n      OAuth 2.0 three-legged (authorization code) flow — the flow every Marketing\n      API call uses. The member consents to the full requested scope set; scopes\n\
  \      cannot be selected individually, and changing an app's scopes forces\n      members to re-authenticate.\n    sources:\n      - openapi/linkedin-ads-openapi.yml\n  - name: OpenIDConnect\n    type: openIdConnect\n    openIdConnectUrl: https://www.linkedin.com/oauth/.well-known/openid-configuration\n    issuer: https://www.linkedin.com/oauth\n    jwks_uri: https://www.linkedin.com/oauth/openid/jwks\n    userinfo_endpoint: https://api.linkedin.com/v2/userinfo\n    id_token_signing_alg_values_supported: [RS256]\n    scopes: [openid, profile, email]\n    description: >-\n      Sign In with LinkedIn using OpenID Connect. Discovery document served live\n      and captured verbatim in well-known/linkedin-ads-openid-configuration.json.\n    sources:\n      - well-known/linkedin-ads-openid-configuration.json\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    description: >-\n\
  \      Two-legged flow, available only to selected partner programs; it grants\n      application-level access with no member context and is not used by the\n      advertising surface.\n    sources:\n      - https://learn.microsoft.com/en-us/linkedin/shared/authentication/client-credentials-flow\ntransport:\n  header: 'Authorization: Bearer {access_token}'\n  bearer_format: opaque (approximately 500 characters; plan for 1000)\ntokens:\n  access_token_ttl_seconds: 5184000\n  access_token_ttl_human: 60 days\n  refresh_token: true\n  refresh_token_note: >-\n    Refresh tokens are longer-lived than access tokens and are returned with\n    refresh_token_expires_in; programmatic refresh is documented.\n  introspection: true\n  introspection_docs: https://learn.microsoft.com/en-us/linkedin/shared/authentication/token-introspection\n  revocation: >-\n    Members can revoke an application's access from their LinkedIn privacy\n    settings; subsequent calls fail 401 and the member must re-authenticate.\n\
  app_registration:\n  portal: https://www.linkedin.com/developers/apps\n  create: https://www.linkedin.com/developers/apps/new\n  credentials: Client ID + Client Secret, per app\n  redirect_uri_rules:\n    - must be absolute HTTPS\n    - query parameters are ignored\n    - fragments (#) are invalid\n  token_generator: https://www.linkedin.com/developers/tools/oauth\n  postman: >-\n    https://www.postman.com/linkedin-developer-apis/workspace/linkedin-marketing-solutions-versioned-apis/overview\nscopes_artifact: scopes/linkedin-ads-scopes.yml\nx-evidence:\n  fetched: '2026-08-13'\n  checks:\n    - url: https://learn.microsoft.com/en-us/linkedin/shared/authentication/authorization-code-flow\n      http_status: 200\n    - url: https://www.linkedin.com/oauth/.well-known/openid-configuration\n      http_status: 200\n    - url: https://learn.microsoft.com/en-us/linkedin/shared/authentication/token-introspection\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/authentication/linkedin-ads-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Advertising
- Marketing
- LinkedIn
- Lead Generation
- Audience Targeting
- Conversions API
- Social Marketing
---
