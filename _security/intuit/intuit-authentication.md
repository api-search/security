---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intuit-customers-api-openapi.yml
  format: yaml
  label: Intuit Customers API
  slug: intuit-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-customers-api-openapi.yml
- filename: intuit-invoices-api-openapi.yml
  format: yaml
  label: Intuit Invoices API
  slug: intuit-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-invoices-api-openapi.yml
- filename: intuit-items-api-openapi.yml
  format: yaml
  label: Intuit Items API
  slug: intuit-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-items-api-openapi.yml
- filename: intuit-payments-api-openapi.yml
  format: yaml
  label: Intuit Payments API
  slug: intuit-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-payments-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Intuit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Intuit secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Intuit
provider_slug: intuit
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    revocationUrl: https://developer.api.intuit.com/v2/oauth2/tokens/revoke
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: oauth2
  scopes: see scopes/intuit-scopes.yml
  source: openapi/_original/quickbooks-accounting.yml
  token_lifetimes:
    access_token: Access tokens are valid for **3,600 seconds** (or one hour).
    refresh_token: Refresh tokens are valid for 100 days.
    refresh_token_hard_limit: Refresh tokens have a hard limit of 5 years.
    refresh_token_rotation: We update the value of the `refresh_token` value every 24 hours hours, or the next time you refresh the access tokens after 24 hours.
  type: oauth2
- jwks_uri: https://oauth.platform.intuit.com/op/v1/jwks
  name: openIdConnect
  note: Endpoints read from the docs and the published discovery document; none of them were called.
  openIdConnectUrl: https://developer.api.intuit.com/.well-known/openid_configuration
  probed:
    http_status: 200
    id_token_signing_alg_values_supported:
    - RS256
    issuer: https://oauth.platform.intuit.com/op/v1
    response_types_supported:
    - code
    scopes_supported:
    - openid
    - email
    - profile
    - address
    - phone
    token_endpoint_auth_methods_supported:
    - client_secret_post
    - client_secret_basic
    url: https://developer.api.intuit.com/.well-known/openid_configuration
  sandbox_openIdConnectUrl: https://developer.api.intuit.com/.well-known/openid_sandbox_configuration
  type: openIdConnect
  userinfo_endpoint: https://accounts.intuit.com/v1/openid_connect/userinfo
slug: intuit-authentication
source_filename: intuit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\nsource: https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization/oauth-2.0\ndocs: https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization\ndocs_pages:\n- https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization/oauth-2.0\n- https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization/openid-connect\n- https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization/oauth-openid-discovery-doc\n- https://developer.intuit.com/quickbooks-online/docs/develop/authentication-and-authorization/faq\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  credentials: Client ID and Client Secret per app, separate Development (sandbox) and Production keys\nschemes:\n- name: oauth2\n  type: oauth2\n  source: openapi/_original/quickbooks-accounting.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n    revocationUrl: https://developer.api.intuit.com/v2/oauth2/tokens/revoke\n  token_lifetimes:\n    access_token: Access tokens are valid for **3,600 seconds** (or one hour).\n    refresh_token: Refresh tokens are valid for 100 days.\n    refresh_token_rotation: We update the value of the `refresh_token` value every 24 hours hours, or the next time you refresh the access tokens after 24 hours.\n    refresh_token_hard_limit: Refresh tokens have a hard limit of 5 years.\n  scopes: see scopes/intuit-scopes.yml\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://developer.api.intuit.com/.well-known/openid_configuration\n  sandbox_openIdConnectUrl: https://developer.api.intuit.com/.well-known/openid_sandbox_configuration\n  probed:\n    url: https://developer.api.intuit.com/.well-known/openid_configuration\n\
  \    http_status: 200\n    issuer: https://oauth.platform.intuit.com/op/v1\n    response_types_supported: [code]\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n    id_token_signing_alg_values_supported: [RS256]\n    scopes_supported: [openid, email, profile, address, phone]\n  userinfo_endpoint: https://accounts.intuit.com/v1/openid_connect/userinfo\n  jwks_uri: https://oauth.platform.intuit.com/op/v1/jwks\n  note: Endpoints read from the docs and the published discovery document; none of them were called.\n"
source_yaml_url: https://artifacts.apis.io/intuit/authentication/intuit-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Accounting
- Custom Fields
- Finance
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Time Tracking
- Fortune 1000
---
