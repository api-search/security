---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ifs-finance-api-openapi.yml
  format: yaml
  label: IFS Finance API
  slug: ifs-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-finance-api-openapi.yml
- filename: ifs-inventory-api-openapi.yml
  format: yaml
  label: IFS Inventory API
  slug: ifs-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-inventory-api-openapi.yml
- filename: ifs-procurement-api-openapi.yml
  format: yaml
  label: IFS Procurement API
  slug: ifs-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-procurement-api-openapi.yml
- filename: ifs-work-orders-api-openapi.yml
  format: yaml
  label: IFS Work Orders API
  slug: ifs-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/openapi/ifs-work-orders-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ifs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- authorizationCode+PKCE
- clientCredentials
- password
overview: IFS secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, authorizationCode+PKCE, clientCredentials, and password flow(s).
provider_name: IFS
provider_slug: ifs
scheme_count: 2
schemes:
- flows:
  - docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/300_client_credential_flow/
    flow: clientCredentials
    parameters:
      client_id: Client ID of the IFS IAM client
      client_secret: Client secret of the IFS IAM client
      grant_type: client_credentials
      scope: openid microprofile-jwt
    use: Applications that cannot render a browser and do not need end-user accounts. Yields an access token for a service user associated with the IAM client itself. Client ID and client secret act as the username and password of the integrating application.
  - docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/100_authorization_code_flow/
    flow: authorizationCode
  - docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/200_authorization_code_flow_pkce/
    flow: authorizationCode+PKCE
  - caution: Legacy flow; IFS documents it but OAuth 2.1 removes it.
    docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/400_resource_owner_pw_credentials/
    flow: password
    name: Resource Owner Password Credentials
  name: IFS IAM (OpenID Connect)
  observed_token_lifetime:
    access_token_expires_in: 180
    note: Values shown in IFS's own documented sample response; actual lifetimes are configured per IAM client.
    refresh_expires_in: 1800
  required_scope: openid microprofile-jwt
  token_endpoint: https://<SYSTEM_URL>/auth/realms/<NAMESPACE>/protocol/openid-connect/token
  token_format: JWT (microprofile-jwt)
  token_response_fields:
  - access_token
  - expires_in
  - refresh_expires_in
  - refresh_token
  - token_type
  - id_token
  - not-before-policy
  - session_state
  - scope
  token_type: Bearer
  type: openIdConnect
- docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/500_basic_authentication_flow/
  name: Basic authentication
  note: '"In IFS Cloud the authentication mechanism is independent from the main/int endpoints (''Compatibility mode'' that was available in Apps 10 is no longer available). In other words, basic authentication is available in both end points but only for ease of upgrade. That means basic authentication is not for the consumption of integrations."'
  scheme: basic
  status: legacy-not-for-integrations
  type: http
slug: ifs-authentication
source_filename: ifs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/\nsupersedes:\n  previous_method: derived\n  previous_source: openapi/ifs-cloud-erp-openapi.yml\n  reason: >-\n    The previous derived profile named authorizationUrl https://login.ifs.cloud/oauth2/authorize\n    and tokenUrl https://login.ifs.cloud/oauth2/token. That host does not resolve (DNS\n    NXDOMAIN, probed 2026-09-13) and IFS does not document it anywhere. The endpoints below\n    are the ones IFS publishes in its own technical documentation.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - authorizationCode+PKCE\n  - clientCredentials\n  - password\n  identity_provider: IFS Identity and Access Manager (IFS IAM) — a Keycloak-shaped OIDC authorization server embedded in the IFS Cloud platform\n  tenancy: >-\n    Every endpoint is tenant-relative.\
  \ IFS Cloud is deployed per customer, so the host is\n    the customer's own IFS Cloud system URL and the realm is that system's namespace.\n    There is no shared, anonymously reachable IFS authorization server.\nschemes:\n- name: IFS IAM (OpenID Connect)\n  type: openIdConnect\n  token_endpoint: https://<SYSTEM_URL>/auth/realms/<NAMESPACE>/protocol/openid-connect/token\n  token_type: Bearer\n  token_format: JWT (microprofile-jwt)\n  required_scope: openid microprofile-jwt\n  token_response_fields:\n  - access_token\n  - expires_in\n  - refresh_expires_in\n  - refresh_token\n  - token_type\n  - id_token\n  - not-before-policy\n  - session_state\n  - scope\n  observed_token_lifetime:\n    access_token_expires_in: 180\n    refresh_expires_in: 1800\n    note: Values shown in IFS's own documented sample response; actual lifetimes are configured per IAM client.\n  flows:\n  - flow: clientCredentials\n    use: >-\n      Applications that cannot render a browser and do not need end-user accounts.\
  \ Yields an\n      access token for a service user associated with the IAM client itself. Client ID and\n      client secret act as the username and password of the integrating application.\n    parameters:\n      grant_type: client_credentials\n      scope: openid microprofile-jwt\n      client_id: Client ID of the IFS IAM client\n      client_secret: Client secret of the IFS IAM client\n    docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/300_client_credential_flow/\n  - flow: authorizationCode\n    docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/100_authorization_code_flow/\n  - flow: authorizationCode+PKCE\n    docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/200_authorization_code_flow_pkce/\n  - flow:\
  \ password\n    name: Resource Owner Password Credentials\n    docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/400_resource_owner_pw_credentials/\n    caution: Legacy flow; IFS documents it but OAuth 2.1 removes it.\n- name: Basic authentication\n  type: http\n  scheme: basic\n  status: legacy-not-for-integrations\n  note: >-\n    \"In IFS Cloud the authentication mechanism is independent from the main/int endpoints\n    ('Compatibility mode' that was available in Apps 10 is no longer available). In other\n    words, basic authentication is available in both end points but only for ease of\n    upgrade. That means basic authentication is not for the consumption of integrations.\"\n  docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/035_iam_clients/020_authenticate_external_integration/500_basic_authentication_flow/\nclient_registration:\n  where: IFS Cloud\
  \ > Solution Manager > Security > Identity and Access Manager > IAM Client Details\n  self_serve: false\n  note: >-\n    A custom IAM client must be registered inside the customer's own IFS Cloud environment by\n    an administrator before an access token can be obtained. There is no public developer\n    signup that yields IFS Cloud API credentials.\nauthorization:\n  model: permission sets\n  note: >-\n    Access to a projection and its entity sets is granted through IFS Cloud permission sets\n    (projection grants, per-projection access levels), plus Access Control Lists applied at\n    projection level. StandardEntity-class APIs additionally require activation by a system\n    administrator before use.\n  docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/020_permission_sets/004_permission_set_overview/010_projections/\nauditing:\n  docs: https://docs.ifs.com/techdocs/26r1/030_administration/010_security/040_iam_settings/080_authentication_auditing/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifs/refs/heads/main/authentication/ifs-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- ERP
- Field Service
- Asset Management
- Manufacturing
- Energy
- Cloud
- Sweden
---
