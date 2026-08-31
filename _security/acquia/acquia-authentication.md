---
api_key_in:
- header
api_specs:
- filename: acquia-account-api-openapi.yml
  format: yaml
  label: Acquia Account API
  slug: acquia-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-account-api-openapi.yml
- filename: acquia-agreements-api-openapi.yml
  format: yaml
  label: Acquia Agreements API
  slug: acquia-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-agreements-api-openapi.yml
- filename: acquia-application-performance-monitoring-services-api-openapi.yml
  format: yaml
  label: Acquia Application Performance Monitoring Services API
  slug: acquia-application-performance-monitoring-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-application-performance-monitoring-services-api-openapi.yml
- filename: acquia-applications-api-openapi.yml
  format: yaml
  label: Acquia Applications API
  slug: acquia-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-applications-api-openapi.yml
- filename: acquia-cloud-ide-api-openapi.yml
  format: yaml
  label: Acquia Cloud IDE API
  slug: acquia-cloud-ide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-ide-api-openapi.yml
- filename: acquia-codebases-api-openapi.yml
  format: yaml
  label: Acquia Codebases API
  slug: acquia-codebases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-codebases-api-openapi.yml
- filename: acquia-current-system-health-api-openapi.yml
  format: yaml
  label: Acquia Current system health API
  slug: acquia-current-system-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-current-system-health-api-openapi.yml
- filename: acquia-distributions-api-openapi.yml
  format: yaml
  label: Acquia Distributions API
  slug: acquia-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-distributions-api-openapi.yml
- filename: acquia-email-api-openapi.yml
  format: yaml
  label: Acquia Email API
  slug: acquia-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-email-api-openapi.yml
- filename: acquia-environments-api-openapi.yml
  format: yaml
  label: Acquia Environments API
  slug: acquia-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-environments-api-openapi.yml
- filename: acquia-identity-providers-api-openapi.yml
  format: yaml
  label: Acquia Identity Providers API
  slug: acquia-identity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-identity-providers-api-openapi.yml
- filename: acquia-invite-api-openapi.yml
  format: yaml
  label: Acquia Invite API
  slug: acquia-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-invite-api-openapi.yml
- filename: acquia-messages-api-openapi.yml
  format: yaml
  label: Acquia Messages API
  slug: acquia-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-messages-api-openapi.yml
- filename: acquia-notifications-api-openapi.yml
  format: yaml
  label: Acquia Notifications API
  slug: acquia-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-notifications-api-openapi.yml
- filename: acquia-options-api-openapi.yml
  format: yaml
  label: Acquia Options API
  slug: acquia-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-options-api-openapi.yml
- filename: acquia-organizations-api-openapi.yml
  format: yaml
  label: Acquia Organizations API
  slug: acquia-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-organizations-api-openapi.yml
- filename: acquia-private-networks-api-openapi.yml
  format: yaml
  label: Acquia Private Networks API
  slug: acquia-private-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-private-networks-api-openapi.yml
- filename: acquia-subscriptions-api-openapi.yml
  format: yaml
  label: Acquia Subscriptions API
  slug: acquia-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-subscriptions-api-openapi.yml
- filename: acquia-teams-and-permissions-api-openapi.yml
  format: yaml
  label: Acquia Teams and Permissions API
  slug: acquia-teams-and-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-teams-and-permissions-api-openapi.yml
- filename: acquia-content-api-openapi.yaml
  format: yaml
  label: Acquia Content API
  slug: acquia-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-content-api-openapi.yaml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Acquia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Acquia secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Acquia
provider_slug: acquia
scheme_count: 2
schemes:
- description: 'All Cloud API calls need to be authenticated in order to work. You authenticate using a token that you can generate on your Acquia Profile page.


    ### To generate a token:


    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and Acquia password.

    2. Click your user avatar in the upper right corner, and then click **Account Settings**.

    3. On the Profile page'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://accounts.acquia.com/api/token
  name: Acquia_Cloud_API_Documentation_OAuth2
  sources:
  - openapi/acquia-account-api-openapi.yml
  - openapi/acquia-agreements-api-openapi.yml
  - openapi/acquia-application-performance-monitoring-services-api-openapi.yml
  - openapi/acquia-applications-api-openapi.yml
  - openapi/acquia-cloud-ide-api-openapi.yml
  - openapi/acquia-codebases-api-openapi.yml
  - openapi/acquia-current-system-health-api-openapi.yml
  - openapi/acquia-distributions-api-openapi.yml
  - openapi/acquia-email-api-openapi.yml
  - openapi/acquia-environments-api-openapi.yml
  - openapi/acquia-identity-providers-api-openapi.yml
  - openapi/acquia-invite-api-openapi.yml
  - openapi/acquia-messages-api-openapi.yml
  - openapi/acquia-notifications-api-openapi.yml
  - openapi/acquia-options-api-openapi.yml
  - openapi/acquia-organizations-api-openapi.yml
  - openapi/acquia-private-networks-api-openapi.yml
  - openapi/acquia-subscriptions-api-openapi.yml
  - openapi/acquia-teams-and-permissions-api-openapi.yml
  type: oauth2
- description: Value for the Authorization header parameter.
  in: header
  name: Codebase_Service_JWT
  parameter: Authorization
  sources:
  - openapi/acquia-account-api-openapi.yml
  - openapi/acquia-agreements-api-openapi.yml
  - openapi/acquia-application-performance-monitoring-services-api-openapi.yml
  - openapi/acquia-applications-api-openapi.yml
  - openapi/acquia-cloud-ide-api-openapi.yml
  - openapi/acquia-codebases-api-openapi.yml
  - openapi/acquia-current-system-health-api-openapi.yml
  - openapi/acquia-distributions-api-openapi.yml
  - openapi/acquia-email-api-openapi.yml
  - openapi/acquia-environments-api-openapi.yml
  - openapi/acquia-identity-providers-api-openapi.yml
  - openapi/acquia-invite-api-openapi.yml
  - openapi/acquia-messages-api-openapi.yml
  - openapi/acquia-notifications-api-openapi.yml
  - openapi/acquia-options-api-openapi.yml
  - openapi/acquia-organizations-api-openapi.yml
  - openapi/acquia-private-networks-api-openapi.yml
  - openapi/acquia-subscriptions-api-openapi.yml
  - openapi/acquia-teams-and-permissions-api-openapi.yml
  type: apiKey
slug: acquia-authentication
source_filename: acquia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: openapi/acquia-account-api-openapi.yml, openapi/acquia-agreements-api-openapi.yml, openapi/acquia-application-performance-monitoring-services-api-openapi.yml,\n  openapi/acquia-applications-api-openapi.yml, openapi/acquia-cloud-ide-api-openapi.yml, openapi/acquia-codebases-api-openapi.yml,\n  openapi/acquia-current-system-health-api-openapi.yml, openapi/acquia-distributions-api-openapi.yml,\n  openapi/acquia-email-api-openapi.yml, openapi/acquia-environments-api-openapi.yml, openapi/acquia-identity-providers-api-openapi.yml,\n  openapi/acquia-invite-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Acquia_Cloud_API_Documentation_OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.acquia.com/api/token\n    scopes: 0\n  description: 'All Cloud API calls need to be authenticated in order\
  \ to work. You authenticate using\n    a token that you can generate on your Acquia Profile page.\n\n\n    ### To generate a token:\n\n\n    1. Sign in to the [Acquia Cloud](https://cloud.acquia.com/) interface using your email address and\n    Acquia password.\n\n    2. Click your user avatar in the upper right corner, and then click **Account Settings**.\n\n    3. On the Profile page'\n  sources:\n  - openapi/acquia-account-api-openapi.yml\n  - openapi/acquia-agreements-api-openapi.yml\n  - openapi/acquia-application-performance-monitoring-services-api-openapi.yml\n  - openapi/acquia-applications-api-openapi.yml\n  - openapi/acquia-cloud-ide-api-openapi.yml\n  - openapi/acquia-codebases-api-openapi.yml\n  - openapi/acquia-current-system-health-api-openapi.yml\n  - openapi/acquia-distributions-api-openapi.yml\n  - openapi/acquia-email-api-openapi.yml\n  - openapi/acquia-environments-api-openapi.yml\n  - openapi/acquia-identity-providers-api-openapi.yml\n  - openapi/acquia-invite-api-openapi.yml\n\
  \  - openapi/acquia-messages-api-openapi.yml\n  - openapi/acquia-notifications-api-openapi.yml\n  - openapi/acquia-options-api-openapi.yml\n  - openapi/acquia-organizations-api-openapi.yml\n  - openapi/acquia-private-networks-api-openapi.yml\n  - openapi/acquia-subscriptions-api-openapi.yml\n  - openapi/acquia-teams-and-permissions-api-openapi.yml\n- name: Codebase_Service_JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Value for the Authorization header parameter.\n  sources:\n  - openapi/acquia-account-api-openapi.yml\n  - openapi/acquia-agreements-api-openapi.yml\n  - openapi/acquia-application-performance-monitoring-services-api-openapi.yml\n  - openapi/acquia-applications-api-openapi.yml\n  - openapi/acquia-cloud-ide-api-openapi.yml\n  - openapi/acquia-codebases-api-openapi.yml\n  - openapi/acquia-current-system-health-api-openapi.yml\n  - openapi/acquia-distributions-api-openapi.yml\n  - openapi/acquia-email-api-openapi.yml\n  - openapi/acquia-environments-api-openapi.yml\n\
  \  - openapi/acquia-identity-providers-api-openapi.yml\n  - openapi/acquia-invite-api-openapi.yml\n  - openapi/acquia-messages-api-openapi.yml\n  - openapi/acquia-notifications-api-openapi.yml\n  - openapi/acquia-options-api-openapi.yml\n  - openapi/acquia-organizations-api-openapi.yml\n  - openapi/acquia-private-networks-api-openapi.yml\n  - openapi/acquia-subscriptions-api-openapi.yml\n  - openapi/acquia-teams-and-permissions-api-openapi.yml\ndocs:\n- https://dev.acquia.com/source-cms/reference/authentication.md\n- https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\n- https://cloudapi-docs.acquia.com/\nsearched_upgrade_note: Upgraded derived -> searched on 2026-08-30. The derived profile saw only the Cloud\n  Platform securitySchemes; the Source CMS OAuth surface below - three grants, published token lifetimes,\n  a 22-scope vocabulary, dynamic client registration and the exact failure diagnostics - is read from\n  Acquia's own authentication reference\
  \ and was absent from every prior round.\nsurfaces:\n- name: Cloud Platform API\n  base_url: https://cloud.acquia.com/api\n  type: oauth2\n  flows:\n  - client_credentials\n  token_url: https://accounts.acquia.com/api/token\n  credential_origin: API key + secret generated by the user at cloud.acquia.com > Account Settings > API\n    Tokens. The secret is displayed once.\n  authorization_model: Teams and Permissions roles, not OAuth scopes\n  scopes: organization:{uuid} only, and only under Federated Authentication\n  docs: https://docs.acquia.com/acquia-cloud-platform/cloud-platform-api-v2-authentication\n- name: Acquia Content API (Source CMS)\n  base_url: '{DRUPAL_SITE_URL}'\n  type: oauth2\n  flows:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  token_url: '{DRUPAL_SITE_URL}/oauth/token'\n  authorize_url: '{DRUPAL_SITE_URL}/oauth/authorize'\n  request_header: 'Authorization: Bearer <token> (exactly one space after Bearer)'\n  token_format: JWT\n  credential_origin:\
  \ API client ID and secret created in the site admin UI at API > API clients; the secret\n    is shown only once.\n  token_lifetimes:\n    access_token_seconds: 300\n    authorization_code_seconds: 300\n    refresh_token_seconds: 1209600\n  refresh_token_availability: Returned only by the authorization_code and refresh_token grants. client_credentials\n    NEVER returns one.\n  scope_count: 22\n  anonymous_access: A site's Public access setting (API > JSON:API) can allow unauthenticated GETs of\n    published content. Unpublished content always requires content:administer.\n  docs: https://dev.acquia.com/source-cms/reference/authentication.md\n- name: Acquia Source MCP server\n  base_url: '{DRUPAL_SITE_URL}/mcp'\n  type: oauth2\n  flows:\n  - client_credentials\n  - authorization_code (via dynamic client registration)\n  dynamic_client_registration: '{DRUPAL_SITE_URL}/oauth/register'\n  discovery:\n  - '{DRUPAL_SITE_URL}/.well-known/oauth-protected-resource'\n  - '{DRUPAL_SITE_URL}/.well-known/oauth-protected-resource/mcp'\n\
  \  - '{DRUPAL_SITE_URL}/.well-known/oauth-authorization-server'\n  - '{DRUPAL_SITE_URL}/.well-known/jwks.json'\n  scopes_supported: 16\n  challenge_gap: The 401 WWW-Authenticate header is only Bearer realm=\"mcp_server\" - it does NOT carry\n    an RFC 9728 resource_metadata parameter, so a client must know the well-known URL out of band.\n  docs: https://dev.acquia.com/source-cms/reference/mcp-server.md\n- name: Acquia identity provider (accounts.acquia.com)\n  type: openIdConnect\n  issuer: https://id.acquia.com/oauth2/default\n  discovery: https://accounts.acquia.com/.well-known/openid-configuration\n  discovery_status: 200\n  saved_to: well-known/acquia-openid-configuration.json\n  grants_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - device_code\n  - CIBA\n  note: Okta-backed. This is the human/SSO identity layer, distinct from the API token surfaces above.\nfailure_diagnostics:\n- condition: expired access token\n  status:\
  \ 401\n  where: WWW-Authenticate header, NOT the body\n  detail: error=\"access_denied\", error_description=\"Access token could not be verified\"\n- condition: malformed token\n  status: 401\n  where: WWW-Authenticate header; the BODY IS HTML, not JSON\n  detail: e.g. Bearer realm=\"OAuth\", error=\"access_denied\", error_description=\"The JWT string must have\n    two dots\"\n- condition: wrong client id or secret\n  status: 401\n  where: JSON body from /oauth/token\n  detail: '{\"error\":\"invalid_client\",\"error_description\":\"Client authentication failed\"}'\n- condition: unknown or unselected scope requested\n  status: 400\n  where: JSON body from /oauth/token; hint names the offending scope\n  detail: '{\"error\":\"invalid_scope\",\"error_description\":\"The requested scope is invalid, unknown, or malformed\"}'\n- condition: valid token missing the needed scope\n  status: 403\n  where: JSON:API error document; detail names the missing permission\n  detail: Existing tokens do NOT\
  \ gain scopes retroactively - select the scope, then request a new token.\ncross_links:\n  scopes: scopes/acquia-scopes.yml\n  conventions: conventions/acquia-conventions.yml\n  errors: errors/acquia-problem-types.yml\n  mcp: mcp/acquia-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/authentication/acquia-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Content
- Experience
- Drupal
- DXP
- CMS
- Digital Asset Management
- Cloud Hosting
- Headless
---
