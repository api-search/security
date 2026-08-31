---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Plotly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plotly declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Plotly
provider_slug: plotly
scheme_count: 4
schemes:
- applies_to:
  - Dash Docs MCP Server (https://dash.plotly.com/_mcp)
  - Plotly Cloud
  bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  discovery:
    oauth_authorization_server: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server
    openid_configuration: https://signin.cloud.plotly.com/.well-known/openid-configuration
    protected_resource_metadata: https://dash.plotly.com/.well-known/oauth-protected-resource/_mcp
  dynamic_client_registration: true
  endpoints:
    authorization: https://signin.cloud.plotly.com/oauth2/authorize
    device_authorization: https://signin.cloud.plotly.com/oauth2/device_authorization
    introspection: https://signin.cloud.plotly.com/oauth2/introspection
    jwks: https://signin.cloud.plotly.com/oauth2/jwks
    registration: https://signin.cloud.plotly.com/oauth2/register
    token: https://signin.cloud.plotly.com/oauth2/token
    userinfo: https://signin.cloud.plotly.com/oauth2/userinfo
  federated_identity:
    note: Plotly Cloud sign-in supports existing accounts such as Google, plus single sign-on for teams (https://dash.plotly.com/plotly-cloud/sign-in).
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id_token_signing_alg:
  - RS256
  issuer: https://signin.cloud.plotly.com
  name: PlotlyCloudOAuth
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_modes:
  - query
  response_types:
  - code
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to:
  - Plotly Cloud CLI (plotly)
  docs: https://dash.plotly.com/plotly-cloud/cli
  env: PLOTLY_API_KEY
  in: cli-flag-or-env
  name: PlotlyCloudApiKey
  note: Non-interactive alternative to `plotly user login`, intended for CI/CD.
  parameter: --api-key
  type: apiKey
- applies_to:
  - Dash Enterprise GraphQL API (https://{dash-enterprise-host}/Manager/graphql)
  docs: https://github.com/plotly/dds-api-docs
  key_source: Dash Enterprise Management UI
  name: DashEnterpriseBasic
  password: DASH_ENTERPRISE_API_KEY / DDS_API_KEY
  rotation:
    note: The resetApiKey GraphQL mutation takes the account password and returns newKey.
    operation: resetApiKey
    supported: true
  scheme: basic
  type: http
  username: DASH_ENTERPRISE_USERNAME / DDS_USERNAME
- applies_to:
  - Dash Enterprise Platform API (via the Dash Enterprise CLI)
  authorization_server: Keycloak (customer-hosted)
  docs: https://dash.plotly.com/dash-enterprise/cli
  login_methods:
  - browser-based flow
  - username and password (recommended for CI/CD)
  name: DashEnterpriseKeycloakOIDC
  note: Self-hosted, so no public discovery document exists to probe. Recorded from Plotly's own documentation.
  protocol: OAuth 2.0 / OpenID Connect
  token_lifetimes:
    access_token: 24 hours (default)
    offline_token_refresh_window: 30 days
  type: openIdConnect
slug: plotly-authentication
source_filename: plotly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://signin.cloud.plotly.com/.well-known/openid-configuration,\n  https://dash.plotly.com/.well-known/oauth-protected-resource/_mcp,\n  https://dash.plotly.com/plotly-cloud/cli, https://dash.plotly.com/dash-enterprise/cli,\n  https://github.com/plotly/dds-api-docs\ndocs: https://dash.plotly.com/plotly-cloud/sign-in\nnote: >-\n  Derived from probed discovery metadata, not from an OpenAPI securitySchemes block - Plotly\n  publishes no OpenAPI. Three distinct auth models operate across three products.\nschemes:\n- name: PlotlyCloudOAuth\n  type: oauth2\n  applies_to:\n  - Dash Docs MCP Server (https://dash.plotly.com/_mcp)\n  - Plotly Cloud\n  issuer: https://signin.cloud.plotly.com\n  discovery:\n    openid_configuration: https://signin.cloud.plotly.com/.well-known/openid-configuration\n    oauth_authorization_server: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server\n    protected_resource_metadata:\
  \ https://dash.plotly.com/.well-known/oauth-protected-resource/_mcp\n  endpoints:\n    authorization: https://signin.cloud.plotly.com/oauth2/authorize\n    token: https://signin.cloud.plotly.com/oauth2/token\n    device_authorization: https://signin.cloud.plotly.com/oauth2/device_authorization\n    introspection: https://signin.cloud.plotly.com/oauth2/introspection\n    userinfo: https://signin.cloud.plotly.com/oauth2/userinfo\n    jwks: https://signin.cloud.plotly.com/oauth2/jwks\n    registration: https://signin.cloud.plotly.com/oauth2/register\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types: [code]\n  response_modes: [query]\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported:\
  \ true\n  bearer_methods_supported: [header]\n  federated_identity:\n    note: >-\n      Plotly Cloud sign-in supports existing accounts such as Google, plus single sign-on for\n      teams (https://dash.plotly.com/plotly-cloud/sign-in).\n- name: PlotlyCloudApiKey\n  type: apiKey\n  in: cli-flag-or-env\n  applies_to:\n  - Plotly Cloud CLI (plotly)\n  parameter: --api-key\n  env: PLOTLY_API_KEY\n  docs: https://dash.plotly.com/plotly-cloud/cli\n  note: Non-interactive alternative to `plotly user login`, intended for CI/CD.\n- name: DashEnterpriseBasic\n  type: http\n  scheme: basic\n  applies_to:\n  - Dash Enterprise GraphQL API (https://{dash-enterprise-host}/Manager/graphql)\n  username: DASH_ENTERPRISE_USERNAME / DDS_USERNAME\n  password: DASH_ENTERPRISE_API_KEY / DDS_API_KEY\n  key_source: Dash Enterprise Management UI\n  rotation:\n    supported: true\n    operation: resetApiKey\n    note: The resetApiKey GraphQL mutation takes the account password and returns newKey.\n  docs: https://github.com/plotly/dds-api-docs\n\
  - name: DashEnterpriseKeycloakOIDC\n  type: openIdConnect\n  applies_to:\n  - Dash Enterprise Platform API (via the Dash Enterprise CLI)\n  authorization_server: Keycloak (customer-hosted)\n  protocol: OAuth 2.0 / OpenID Connect\n  token_lifetimes:\n    access_token: 24 hours (default)\n    offline_token_refresh_window: 30 days\n  login_methods:\n  - browser-based flow\n  - username and password (recommended for CI/CD)\n  docs: https://dash.plotly.com/dash-enterprise/cli\n  note: >-\n    Self-hosted, so no public discovery document exists to probe. Recorded from Plotly's own\n    documentation.\napp_level_auth:\n  note: >-\n    Distinct from provider authentication: Plotly ships auth libraries its customers embed in\n    their own Dash apps - dash-auth (basic auth and Plotly authentication) and\n    dash-enterprise-auth. Dash MCP servers running inside a customer app either inherit Plotly\n    Cloud authentication or implement the standard OAuth 2.0 flow from the MCP specification\n  \
  \  (https://dash.plotly.com/dash-mcp/auth).\nx-evidence:\n- url: https://signin.cloud.plotly.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://signin.cloud.plotly.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://dash.plotly.com/.well-known/oauth-protected-resource/_mcp\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotly/refs/heads/main/authentication/plotly-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Data Visualization
- Analytics
- Data Apps
- Business Intelligence
- Open-Source
- Python
- JavaScript
- Charts
- Dashboards
- Developer Tools
- MCP
---
