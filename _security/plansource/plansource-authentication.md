---
api_key_in:
- header
api_specs:
- filename: plansource-aca-api-openapi.yml
  format: yaml
  label: PlanSource ACA API
  slug: plansource-aca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-aca-api-openapi.yml
- filename: plansource-administrators-api-openapi.yml
  format: yaml
  label: PlanSource Administrators API
  slug: plansource-administrators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-administrators-api-openapi.yml
- filename: plansource-collections-api-openapi.yml
  format: yaml
  label: PlanSource Collections API
  slug: plansource-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-collections-api-openapi.yml
- filename: plansource-coverage-api-openapi.yml
  format: yaml
  label: PlanSource Coverage API
  slug: plansource-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-coverage-api-openapi.yml
- filename: plansource-demographic-api-openapi.yml
  format: yaml
  label: PlanSource Demographic API
  slug: plansource-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-demographic-api-openapi.yml
- filename: plansource-eoi-api-openapi.yml
  format: yaml
  label: PlanSource EOI API
  slug: plansource-eoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-eoi-api-openapi.yml
- filename: plansource-page-content-api-openapi.yml
  format: yaml
  label: PlanSource Page Content API
  slug: plansource-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-page-content-api-openapi.yml
- filename: plansource-payroll-api-openapi.yml
  format: yaml
  label: PlanSource Payroll API
  slug: plansource-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-payroll-api-openapi.yml
- filename: plansource-security-api-openapi.yml
  format: yaml
  label: PlanSource Security API
  slug: plansource-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-security-api-openapi.yml
auth_types:
- oauth2
- apiKey
- openIdConnect
- saml2
description: ''
kind: authentication
layout: security
method: searched
name: Plansource Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: PlanSource secures its APIs with oauth2, apiKey, openIdConnect, and saml2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: PlanSource
provider_slug: plansource
scheme_count: 5
schemes:
- flows:
  - flow: clientCredentials
    partner_dev_tokenUrl: https://partner-dev-api.plansource.com/oauth/v2/token
    scopes: 1
    tokenUrl: https://api.plansource.com/oauth/v2/token
  name: clientSecretJwt
  preferred: true
  sources:
  - openapi/plansource-admin-api-openapi-original.json
  surface: Admin API
  type: oauth2
- in: header
  name: authString
  note: Legacy scheme. Required together with the Signature header - the spec's second security requirement lists both, so neither header authenticates on its own.
  parameter: AuthenticationString
  sources:
  - openapi/plansource-admin-api-openapi-original.json
  surface: Admin API
  type: apiKey
- in: header
  name: signature
  note: Request-signature companion to AuthenticationString.
  parameter: Signature
  sources:
  - openapi/plansource-admin-api-openapi-original.json
  surface: Admin API
  type: apiKey
- authorization_endpoint: https://api.plansource.com/sso/oauth2/authorize
  deviations:
  - issuer is ".plansource.com", not an https URL
  - jwks_uri holds an inline JWK object instead of a URI
  - claim_types_supported is a string, not an array
  discovery: https://api.plansource.com/.well-known/openid-configuration
  grant_types_supported:
  - code
  id_token_signing_alg_values_supported:
  - RS256
  name: plansource-sso-oidc
  response_types_supported:
  - token id_token
  sources:
  - well-known/plansource-openid-configuration.json
  surface: end-user SSO
  token_endpoint: https://api.plansource.com/sso/oauth2/token
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://api.plansource.com/sso/oauth2/user_info
- docs: https://developer.plansource.com/docs/saml-20-sso-implementation
  name: plansource-sso-saml2
  note: SAMLResponse / RelayState / Cookie appear as explicit header parameters on the SSO operations in the spec.
  sources:
  - openapi/plansource-admin-api-openapi-original.json
  - https://developer.plansource.com/docs/saml-20-sso-implementation
  surface: end-user SSO
  type: saml2
slug: plansource-authentication
source_filename: plansource-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource:\n- openapi/plansource-admin-api-openapi-original.json\n- https://api.plansource.com/.well-known/openid-configuration\n- https://developer.plansource.com/docs/saml-20-sso-implementation\n- https://developer.plansource.com/docs/utilize-postman\ndocs: https://developer.plansource.com/v2.0/reference\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - openIdConnect\n  - saml2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  note: 'Two distinct auth surfaces: machine-to-machine for the Admin API (client credentials / header\n    pair), and end-user SSO for the employee and admin portals (OIDC authorization code, or SAML 2.0).'\nschemes:\n- name: clientSecretJwt\n  type: oauth2\n  surface: Admin API\n  preferred: true\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.plansource.com/oauth/v2/token\n    partner_dev_tokenUrl: https://partner-dev-api.plansource.com/oauth/v2/token\n\
  \    scopes: 1\n  sources:\n  - openapi/plansource-admin-api-openapi-original.json\n- name: authString\n  type: apiKey\n  in: header\n  parameter: AuthenticationString\n  surface: Admin API\n  note: Legacy scheme. Required together with the Signature header - the spec's second security requirement\n    lists both, so neither header authenticates on its own.\n  sources:\n  - openapi/plansource-admin-api-openapi-original.json\n- name: signature\n  type: apiKey\n  in: header\n  parameter: Signature\n  surface: Admin API\n  note: Request-signature companion to AuthenticationString.\n  sources:\n  - openapi/plansource-admin-api-openapi-original.json\n- name: plansource-sso-oidc\n  type: openIdConnect\n  surface: end-user SSO\n  discovery: https://api.plansource.com/.well-known/openid-configuration\n  authorization_endpoint: https://api.plansource.com/sso/oauth2/authorize\n  token_endpoint: https://api.plansource.com/sso/oauth2/token\n  userinfo_endpoint: https://api.plansource.com/sso/oauth2/user_info\n\
  \  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  id_token_signing_alg_values_supported:\n  - RS256\n  grant_types_supported:\n  - code\n  response_types_supported:\n  - token id_token\n  sources:\n  - well-known/plansource-openid-configuration.json\n  deviations:\n  - issuer is \".plansource.com\", not an https URL\n  - jwks_uri holds an inline JWK object instead of a URI\n  - claim_types_supported is a string, not an array\n- name: plansource-sso-saml2\n  type: saml2\n  surface: end-user SSO\n  docs: https://developer.plansource.com/docs/saml-20-sso-implementation\n  note: SAMLResponse / RelayState / Cookie appear as explicit header parameters on the SSO operations\n    in the spec.\n  sources:\n  - openapi/plansource-admin-api-openapi-original.json\n  - https://developer.plansource.com/docs/saml-20-sso-implementation\ncredential_issuance:\n  self_serve: false\n  note: API credentials (lookup_code, plansource_admin, secret) are provisioned by PlanSource, not self-issued.\n\
  \    Partners request them through their PlanSource administrator contact or dev.support@plansource.com.\n  contact: dev.support@plansource.com\nmcp:\n  url: https://developer.plansource.com/mcp\n  scheme: OAuth 2.0\n  protected_resource_metadata: https://developer.plansource.com/.well-known/oauth-protected-resource/mcp\n  authorization_servers:\n  - https://dash.readme.com/oidc\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/authentication/plansource-authentication.yml
summary_line: oauth2/apiKey/openIdConnect/saml2 · 5 schemes
tags:
- Employee Benefits
- Benefits Administration
- Insurance
- Human Resources
- Payroll
- Health Insurance
- Enrollment
- HR Technology
- Evidence of Insurability
- ACA Reporting
- Eligibility
- Single Sign-On
---
