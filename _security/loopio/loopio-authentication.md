---
api_key_in: []
api_specs:
- filename: loopio-asynchronous-api-openapi.yml
  format: yaml
  label: Loopio Asynchronous API
  slug: loopio-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-asynchronous-api-openapi.yml
- filename: loopio-crm-api-openapi.yml
  format: yaml
  label: Loopio CRM API
  slug: loopio-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-crm-api-openapi.yml
- filename: loopio-custom-project-fields-api-openapi.yml
  format: yaml
  label: Loopio Custom Project Fields API
  slug: loopio-custom-project-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-custom-project-fields-api-openapi.yml
- filename: loopio-customers-api-openapi.yml
  format: yaml
  label: Loopio Customers API
  slug: loopio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-customers-api-openapi.yml
- filename: loopio-files-api-openapi.yml
  format: yaml
  label: Loopio Files API
  slug: loopio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-files-api-openapi.yml
- filename: loopio-library-entries-api-openapi.yml
  format: yaml
  label: Loopio Library Entries API
  slug: loopio-library-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-library-entries-api-openapi.yml
- filename: loopio-merge-variables-api-openapi.yml
  format: yaml
  label: Loopio Merge Variables API
  slug: loopio-merge-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-merge-variables-api-openapi.yml
- filename: loopio-project-templates-api-openapi.yml
  format: yaml
  label: Loopio Project Templates API
  slug: loopio-project-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-project-templates-api-openapi.yml
- filename: loopio-projects-api-openapi.yml
  format: yaml
  label: Loopio Projects API
  slug: loopio-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-projects-api-openapi.yml
- filename: loopio-roles-api-openapi.yml
  format: yaml
  label: Loopio Roles API
  slug: loopio-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-roles-api-openapi.yml
- filename: loopio-stacks-api-openapi.yml
  format: yaml
  label: Loopio Stacks API
  slug: loopio-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-stacks-api-openapi.yml
- filename: loopio-tags-api-openapi.yml
  format: yaml
  label: Loopio Tags API
  slug: loopio-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-tags-api-openapi.yml
- filename: loopio-teams-api-openapi.yml
  format: yaml
  label: Loopio Teams API
  slug: loopio-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-teams-api-openapi.yml
- filename: loopio-users-api-openapi.yml
  format: yaml
  label: Loopio Users API
  slug: loopio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-users-api-openapi.yml
- filename: loopio-webhooks-api-openapi.yml
  format: yaml
  label: Loopio Webhooks API
  slug: loopio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/openapi/loopio-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Loopio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Loopio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Loopio
provider_slug: loopio
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.loopio.com/oauth2/authorize
    flow: authorizationCode
    scopes_in_spec: 22
    tokenUrl: https://api.loopio.com/oauth2/access_token
  - flow: clientCredentials
    scopes_in_spec: 22
    tokenUrl: https://api.loopio.com/oauth2/access_token
  in_spec: true
  name: loopio_auth
  sources:
  - openapi/loopio-openapi.yaml
  type: oauth2
slug: loopio-authentication
source_filename: loopio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://developer.loopio.com/docs/loopio-api/c56ffe1fdae3e-getting-started-with-the-loopio-api\ndocs: https://developer.loopio.com/docs/loopio-api/c56ffe1fdae3e-getting-started-with-the-loopio-api\nderived_from:\n- openapi/loopio-openapi.yaml\n- well-known/loopio-oauth-authorization-server.json\n- well-known/loopio-oauth-protected-resource.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  primary_flow: clientCredentials\n  bearer_methods_supported:\n  - header\n  note: >-\n    The published OpenAPI declares both an authorizationCode and a clientCredentials flow,\n    and the RFC 8414 discovery document additionally advertises refresh_token. The Getting\n    Started guide states plainly that \"clients are authenticated using the client_credentials\n    flow\", so client credentials is the documented path for API integrations.\nschemes:\n- name: loopio_auth\n  type: oauth2\n\
  \  in_spec: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.loopio.com/oauth2/authorize\n    tokenUrl: https://api.loopio.com/oauth2/access_token\n    scopes_in_spec: 22\n  - flow: clientCredentials\n    tokenUrl: https://api.loopio.com/oauth2/access_token\n    scopes_in_spec: 22\n  sources:\n  - openapi/loopio-openapi.yaml\nauthorization_server:\n  issuer: https://api.loopio.com\n  metadata_document: https://api.loopio.com/.well-known/oauth-authorization-server\n  metadata_status: 200\n  authorization_endpoint: https://api.loopio.com/oauth2/authorize\n  token_endpoint: https://api.loopio.com/oauth2/access_token\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  code_challenge_methods_supported:\n  - S256\n  client_id_metadata_document_supported:\
  \ true\n  op_policy_uri: https://loopio.com/legal/privacy/\n  op_tos_uri: https://loopio.com/legal/\nprotected_resource:\n  metadata_document: https://api.loopio.com/.well-known/oauth-protected-resource\n  metadata_status: 200\n  resource: https://api.loopio.com\n  resource_name: Loopio\n  authorization_servers:\n  - https://api.loopio.com\n  bearer_methods_supported:\n  - header\ntoken_request:\n  method: POST\n  url: https://api.loopio.com/oauth2/access_token\n  content_type: application/x-www-form-urlencoded\n  parameters:\n  - grant_type=client_credentials\n  - scope (space-delimited, URL-encoded as +)\n  - client_id\n  - client_secret\n  response_fields:\n  - token_type\n  - expires_in\n  - access_token\n  token_type: Bearer\n  expires_in_seconds: 3600\n  request_header: 'Authorization: Bearer {token}'\ncredential_lifecycle:\n  issued_by: A Loopio Admin creates an App under Admin > Integrations > For Developers\n  secret_visibility: The client secret is shown once, only while the\
  \ admin remains on the creation page\n  scope_mutability: >-\n    Scopes cannot be changed after an App is created — the App must be deleted and recreated\n    with a different scope set.\n  guidance: Loopio's docs direct integrators to the principle of least privilege when selecting scopes\nregions:\n- name: North America\n  host: https://api.loopio.com\n  status: available\n- name: Europe\n  host: https://api.eu.loopio.com\n  status: >-\n    declared in the OpenAPI servers[] block but the Getting Started guide carries an explicit\n    disclaimer that \"the European API hasn't been made accessible yet. At this time please\n    only use api.loopio.com host.\"\n- name: int01 test instances\n  host: https://api.int01.loopio.com\n  status: separate credentials required; provisioned by Loopio, not self-serve\nnotes:\n- Credentials are datacenter-scoped — a client issued for North America will not work in Europe.\n- No API-key, HTTP basic, mutualTLS or openIdConnect scheme is declared anywhere\
  \ in the contract.\n- No /.well-known/openid-configuration is served; OIDC discovery returns 404 on api.loopio.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopio/refs/heads/main/authentication/loopio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- RFP
- Proposals
- Response Management
- Content Library
- Sales Enablement
- Questionnaires
- Compliance
- Collaboration
- Documents
- Webhooks
- SaaS
---
