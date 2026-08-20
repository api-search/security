---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Western Alliance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Western Alliance Bank secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Western Alliance Bank
provider_slug: western-alliance
scheme_count: 3
schemes:
- applies_to: Western Alliance Bank Treasury Management open-banking API
  credentials:
  - Client ID
  - Client Secret
  - access Token (issued by the API gateway)
  evidence: API Services Terms & Conditions define "API Authentication Credentials" as Client ID + Client Secret + Client Certificate + Token, i.e. OAuth2 client-credentials with a token issued per environment (UAT / Production).
  flow: clientCredentials
  name: TreasuryManagementOAuth2
  type: oauth2
- applies_to: Western Alliance Bank Treasury Management open-banking API
  evidence: A Client Certificate (mutual TLS) is a required component of the API Authentication Credentials alongside the OAuth2 client-credentials pair.
  name: TreasuryManagementClientCertificate
  type: mutualTLS
- applies_to: WAB Developer Hub portal login (Salesforce Experience Cloud IdP) — not the business API
  authorization_endpoint: https://developer.westernalliancebank.com/services/oauth2/authorize
  evidence: /.well-known/openid-configuration returns 200 anonymously.
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://developer.westernalliancebank.com/services/oauth2/introspect
  issuer: https://developer.westernalliancebank.com
  jwks_uri: https://developer.westernalliancebank.com/id/keys
  name: DeveloperHubPortalOIDC
  revocation_endpoint: https://developer.westernalliancebank.com/services/oauth2/revoke
  source: well-known/western-alliance-openid-configuration.json
  token_endpoint: https://developer.westernalliancebank.com/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: western-alliance-authentication
source_filename: western-alliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  API Services Terms & Conditions (https://www.westernalliancebancorporation.com/sites/default/files/2025-05/api-services-terms-conditions.pdf)\n  + /.well-known/openid-configuration on the WAB Developer Hub\ndocs: https://developer.westernalliancebank.com/s/\nnote: >-\n  No public OpenAPI is downloadable (the Treasury Management API spec is\n  credential-gated behind the WAB Developer Hub), so this profile is derived from\n  the provider's published API Services Terms & Conditions and the anonymously\n  served OIDC discovery document — not from a harvested securitySchemes block.\nsummary:\n  types: [oauth2, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  mtls: true\n  environments: [UAT, Production]\nschemes:\n- name: TreasuryManagementOAuth2\n  type: oauth2\n  applies_to: Western Alliance Bank Treasury Management open-banking API\n  flow: clientCredentials\n  credentials:\n  - Client ID\n  - Client Secret\n  - access\
  \ Token (issued by the API gateway)\n  evidence: >-\n    API Services Terms & Conditions define \"API Authentication Credentials\" as\n    Client ID + Client Secret + Client Certificate + Token, i.e. OAuth2\n    client-credentials with a token issued per environment (UAT / Production).\n- name: TreasuryManagementClientCertificate\n  type: mutualTLS\n  applies_to: Western Alliance Bank Treasury Management open-banking API\n  evidence: >-\n    A Client Certificate (mutual TLS) is a required component of the API\n    Authentication Credentials alongside the OAuth2 client-credentials pair.\n- name: DeveloperHubPortalOIDC\n  type: openIdConnect\n  applies_to: WAB Developer Hub portal login (Salesforce Experience Cloud IdP) — not the business API\n  issuer: https://developer.westernalliancebank.com\n  authorization_endpoint: https://developer.westernalliancebank.com/services/oauth2/authorize\n  token_endpoint: https://developer.westernalliancebank.com/services/oauth2/token\n  introspection_endpoint:\
  \ https://developer.westernalliancebank.com/services/oauth2/introspect\n  revocation_endpoint: https://developer.westernalliancebank.com/services/oauth2/revoke\n  jwks_uri: https://developer.westernalliancebank.com/id/keys\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg_values_supported: [RS256]\n  source: well-known/western-alliance-openid-configuration.json\n  evidence: /.well-known/openid-configuration returns 200 anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-alliance/refs/heads/main/authentication/western-alliance-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Financial-Services
- Banking
- United States
- Treasury Management
- Open Banking
- Payments
- Commercial Banking
---
