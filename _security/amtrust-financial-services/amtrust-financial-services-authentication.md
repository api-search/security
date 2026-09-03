---
api_key_in:
- header
- query
api_specs:
- filename: amtrust-financial-services-digital-wc-api-openapi.json
  format: json
  label: AmTrust Digital WC API
  slug: amtrust-financial-services-digital-wc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-wc-api-openapi.json
- filename: amtrust-financial-services-digital-bop-api-openapi.json
  format: json
  label: AmTrust Digital BOP API
  slug: amtrust-financial-services-digital-bop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-bop-api-openapi.json
- filename: amtrust-financial-services-digital-cyber-api-openapi.json
  format: json
  label: AmTrust Digital Cyber API
  slug: amtrust-financial-services-digital-cyber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-cyber-api-openapi.json
- filename: amtrust-financial-services-digital-es-api-openapi.json
  format: json
  label: AmTrust Digital E&S API
  slug: amtrust-financial-services-digital-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-es-api-openapi.json
- filename: amtrust-financial-services-digital-pac-api-openapi.json
  format: json
  label: AmTrust Digital PAC API
  slug: amtrust-financial-services-digital-pac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-pac-api-openapi.json
- filename: amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
  format: json
  label: AmTrust Reinsurance Contract Entry API
  slug: amtrust-financial-services-reinsurance-contract-entry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
- filename: amtrust-financial-services-experience-claims-medical-case-api-openapi.json
  format: json
  label: AmTrust Experience Claims Medical Case API
  slug: amtrust-financial-services-experience-claims-medical-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json
- filename: amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
  format: json
  label: AmTrust Experience Next Gen Bond Pro API
  slug: amtrust-financial-services-experience-next-gen-bond-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
- filename: amtrust-financial-services-conversa-engine-api-openapi.json
  format: json
  label: AmTrust Conversa Engine API
  slug: amtrust-financial-services-conversa-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-conversa-engine-api-openapi.json
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Amtrust Financial Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: AmTrust Financial Services secures its APIs with apiKey and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
scheme_count: 4
schemes:
- description: 'Azure API Management subscription key. Issued per subscriber after the partner vetting process. Confirmed live: the gateway answers an unauthenticated call with `WWW-Authenticate: AzureApiManagementKey realm="https://gateway.amtrustgroup.com/digital-bop",name="subscriber_id",type="header"`.'
  in: header
  name: apiKeyHeader
  parameter: subscriber_id
  sources:
  - openapi/amtrust-financial-services-conversa-engine-api-openapi.json
  - openapi/amtrust-financial-services-digital-bop-api-openapi.json
  - openapi/amtrust-financial-services-digital-cyber-api-openapi.json
  - openapi/amtrust-financial-services-digital-es-api-openapi.json
  - openapi/amtrust-financial-services-digital-pac-api-openapi.json
  - openapi/amtrust-financial-services-digital-wc-api-openapi.json
  - openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json
  - openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
  - openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
  type: apiKey
- description: Same subscription key passed as a query parameter instead of a header. Discouraged.
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/amtrust-financial-services-digital-bop-api-openapi.json
  - openapi/amtrust-financial-services-digital-cyber-api-openapi.json
  - openapi/amtrust-financial-services-digital-es-api-openapi.json
  - openapi/amtrust-financial-services-digital-pac-api-openapi.json
  - openapi/amtrust-financial-services-digital-wc-api-openapi.json
  - openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json
  - openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
  - openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
  type: apiKey
- description: The Conversa Engine API alone names its query-string key `subscriber_id` rather than `subscription-key` — an inconsistency across the estate.
  in: query
  name: apiKeyQueryConversa
  parameter: subscriber_id
  sources:
  - openapi/amtrust-financial-services-conversa-engine-api-openapi.json
  type: apiKey
- description: 'AmTrust IdentityServer bearer token, sent as `Authorization: Bearer <access token>` alongside the subscription key. NOT declared in any OpenAPI securityScheme — documented only on the portal.'
  name: amtrustIdentityServer
  openIdConnectUrl: https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration
  sources:
  - https://apiportal.amtrustgroup.com/authentication
  - https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration
  type: openIdConnect
slug: amtrust-financial-services-authentication
source_filename: amtrust-financial-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://apiportal.amtrustgroup.com/authentication (HTTP 200),\n  https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration (HTTP 200),\n  https://uatauth.amtrustgroup.com/AuthServer_usertest/.well-known/openid-configuration (HTTP 200),\n  a live 401 from https://gateway.amtrustgroup.com/digital-bop/api/v1/agent-contacts, and the nine\n  harvested OpenAPI documents in openapi/ — probed 2026-09-02\ndocs: https://apiportal.amtrustgroup.com/authentication\nsummary:\n  model: two-factor gateway — an Azure API Management subscription key AND an OpenID Connect bearer token\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  - query\nnote: >-\n  AmTrust requires BOTH credentials on every call and the OpenAPI documents only describe one of them.\n  The specs declare the APIM subscription key (`subscriber_id` header / `subscription-key` query) and\n  nothing else; the bearer token from AmTrust's\
  \ IdentityServer is documented only on the portal\n  authentication page. An integrator working from the machine-readable contract alone would build a\n  client that 401s. This gap is the single most consequential thing in AmTrust's auth surface.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: subscriber_id\n  description: >-\n    Azure API Management subscription key. Issued per subscriber after the partner vetting process.\n    Confirmed live: the gateway answers an unauthenticated call with\n    `WWW-Authenticate: AzureApiManagementKey realm=\"https://gateway.amtrustgroup.com/digital-bop\",name=\"subscriber_id\",type=\"header\"`.\n  sources:\n  - openapi/amtrust-financial-services-conversa-engine-api-openapi.json\n  - openapi/amtrust-financial-services-digital-bop-api-openapi.json\n  - openapi/amtrust-financial-services-digital-cyber-api-openapi.json\n  - openapi/amtrust-financial-services-digital-es-api-openapi.json\n  - openapi/amtrust-financial-services-digital-pac-api-openapi.json\n\
  \  - openapi/amtrust-financial-services-digital-wc-api-openapi.json\n  - openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json\n  - openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json\n  - openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  description: Same subscription key passed as a query parameter instead of a header. Discouraged.\n  sources:\n  - openapi/amtrust-financial-services-digital-bop-api-openapi.json\n  - openapi/amtrust-financial-services-digital-cyber-api-openapi.json\n  - openapi/amtrust-financial-services-digital-es-api-openapi.json\n  - openapi/amtrust-financial-services-digital-pac-api-openapi.json\n  - openapi/amtrust-financial-services-digital-wc-api-openapi.json\n  - openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json\n  - openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json\n\
  \  - openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json\n- name: apiKeyQueryConversa\n  type: apiKey\n  in: query\n  parameter: subscriber_id\n  description: >-\n    The Conversa Engine API alone names its query-string key `subscriber_id` rather than\n    `subscription-key` — an inconsistency across the estate.\n  sources:\n  - openapi/amtrust-financial-services-conversa-engine-api-openapi.json\n- name: amtrustIdentityServer\n  type: openIdConnect\n  openIdConnectUrl: https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration\n  description: >-\n    AmTrust IdentityServer bearer token, sent as `Authorization: Bearer <access token>` alongside the\n    subscription key. NOT declared in any OpenAPI securityScheme — documented only on the portal.\n  sources:\n  - https://apiportal.amtrustgroup.com/authentication\n  - https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration\nidentity_provider:\n  vendor: IdentityServer (self-hosted\
  \ by AmTrust)\n  environments:\n  - environment: production\n    issuer: https://auth.amtrustgroup.com/AuthServer\n    discovery: https://auth.amtrustgroup.com/AuthServer/.well-known/openid-configuration\n    token_endpoint: https://auth.amtrustgroup.com/AuthServer/OpenIDConnect/Token\n    jwks_uri: https://auth.amtrustgroup.com/AuthServer/.well-known/jwks\n    status: 200\n  - environment: uat\n    issuer: https://uatauth.amtrustgroup.com/AuthServer_usertest\n    discovery: https://uatauth.amtrustgroup.com/AuthServer_usertest/.well-known/openid-configuration\n    token_endpoint: https://uatauth.amtrustgroup.com/AuthServer_usertest/OpenIDConnect/Token\n    jwks_uri: https://uatauth.amtrustgroup.com/AuthServer_usertest/.well-known/jwks\n    status: 200\n  grant_types_supported:\n  - client_credentials\n  - token_exchange\n  - authorization_code\n  - refresh_token\n  - password\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n\
  \  - RS256\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_lifetime: 4 hours (documented on the portal authentication page; tokens are reusable within\n    that window)\n  flows:\n  - name: General Access Token\n    grant_type: client_credentials\n    scope: openid profile\n    use: APIs that do not need a user identity\n  - name: User Authenticated Token\n    grant_type: password\n    scope: openid profile legacy_info legacy_id\n    use: APIs that act on behalf of a named portal user\n  required_headers:\n  - Content-Type: application/x-www-form-urlencoded (on the token request)\n  - Authorization: Bearer <access token>\n  - subscriber_id: <subscriber_id>\ngaps:\n- >-\n  No securityScheme of type oauth2 or openIdConnect appears in any of the nine OpenAPI documents,\n  so the bearer-token half of the contract is invisible to code generators and agents.\n- >-\n  `plain` is advertised in code_challenge_methods_supported alongside S256, which permits a PKCE\n  downgrade\
  \ for any public client using the authorization_code flow.\n- >-\n  The `password` (resource owner password credentials) grant is enabled in production. OAuth 2.1\n  removes it and RFC 9700 (BCP for OAuth 2.0 Security) explicitly says it MUST NOT be used.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/authentication/amtrust-financial-services-authentication.yml
summary_line: apiKey/openIdConnect · 4 schemes
tags:
- Commercial Insurance
- Insurance
- Property and Casualty
- Small Business
- Workers Compensation
- Fortune 1000
- Underwriting
- Claims
- Policy
- Reinsurance
- Cyber Insurance
- Surety
---
