---
api_key_in: []
api_specs:
- filename: switstack-switcloud-openapi.yml
  format: yaml
  label: Switcloud API
  slug: switcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-switcloud-openapi.yml
- filename: switstack-swittest-openapi.yml
  format: yaml
  label: Swittest API
  slug: swittest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-swittest-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Switstack Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
overview: Switstack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and clientCredentials flow(s).
provider_name: Switstack
provider_slug: switstack
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: auth/token
  - flow: clientCredentials
    scopes: 0
    source: https://docs.switstack.io/switcloud/security_authentication/
    tokenUrl: auth/token
  name: OAuth2PasswordBearer
  sources:
  - openapi/switstack-switcloud-openapi.yml
  - openapi/switstack-swittest-openapi.yml
  type: oauth2
slug: switstack-authentication
source_filename: switstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/switstack-switcloud-openapi.yml, openapi/switstack-swittest-openapi.yml\ndocs: https://docs.switstack.io/switcloud/security_authentication/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  - clientCredentials\n  bearer: true\n  authorization_header: 'Authorization: Bearer <access_token>'\n  note: >-\n    Both published Switstack APIs use the same FastAPI-generated OAuth2 password-bearer scheme. The OpenAPI declares\n    only the password flow; the Switcloud security & authentication docs additionally document a client-credentials\n    grant for machine users. No API-key, basic, mutualTLS or OpenID Connect scheme is published.\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: auth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: auth/token\n    scopes: 0\n    source: https://docs.switstack.io/switcloud/security_authentication/\n  sources:\n\
  \  - openapi/switstack-switcloud-openapi.yml\n  - openapi/switstack-swittest-openapi.yml\ntoken_endpoints:\n- api: Switcloud API\n  spec_path: /auth/token\n  documented_url: https://switcloud.switstack.io/api/oauth/token\n  grant_types:\n  - password\n  - client_credentials\n  request_schema: OAuth2Form\n  response_schema: TokenSchema\n  response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  token_type: bearer\n  expires_in_seconds: 3600\n  source: https://docs.switstack.io/switcloud/security_authentication/\n  note: >-\n    The docs example posts to https://switcloud.switstack.io/api/oauth/token while OpenAPI 2.28.0 declares\n    /auth/token; the two disagree and the documented host does not resolve in public DNS (see\n    lifecycle/switstack-lifecycle.yml). Recorded as published, not reconciled.\n- api: Swittest API\n  spec_path: /auth/token\n  grant_types:\n  - password\n  request_schema: OAuth2Form\n  response_schema: TokenSchema\n  token_type: bearer\n  source: openapi/switstack-swittest-openapi.yml\n\
  token_lifecycle:\n- operation: token\n  path: /auth/token\n  purpose: Issue an access token\n- operation: refresh_token\n  path: /auth/refresh-token\n  purpose: Exchange a refresh token for a new access token\n- operation: revoke_token\n  path: /auth/revoke-token\n  purpose: Revoke an issued token\nauthorization_model:\n  style: role-based\n  note: >-\n    Access control is expressed as named roles, not OAuth scopes; the OpenAPI flow declares an empty scopes map.\n  switcloud_roles:\n  - name: Super Admin\n    description: Manages the entire system (CRUD on all models); Payment data is read-only.\n  - name: Organization Admin\n    description: >-\n      Manages users, merchants, stores and POI configurations within their own organization; cannot see other\n      organizations' data and cannot create payments.\n  - name: Basic user (human or machine)\n    description: Read-only on their organization's data; can create and update Payments.\n  swittest_roles:\n  - name: Data\n    description:\
  \ Can get test suites, tests, configs and vcards.\n  - name: Full\n    description: Can fully use Swittest.\n  source: https://docs.switstack.io/switcloud/security_authentication/\nonboarding:\n  self_serve: false\n  note: >-\n    Credentials are not self-serve. Switcloud getting-started requires \"Access to the Switcloud API sandbox\" and\n    \"Access to the Switstack packages repository\" and directs the reader to contact Switstack sales or support;\n    Swittest instances are provisioned per customer/partner by a Switstack representative. Account requests go to\n    contact@switstack.io.\n  evidence:\n  - url: https://docs.switstack.io/switcloud/getting_started/\n    status: 200\n  - url: https://docs.switstack.io/swittest/setup/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/authentication/switstack-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech Insurtech
- payments
- emv
- emv-level-2
- card-present
- point-of-sale
- softpos
- tap-to-pay
- payment-terminals
- in-store-payments
- pci-mpoc
- certification-testing
- retail-payments
- estate-management
---
