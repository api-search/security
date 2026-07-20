---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Genentech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Genentech secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Genentech
provider_slug: genentech
scheme_count: 3
schemes:
- issuer: https://developer.gene.com
  name: openIdConnect
  openIdConnectUrl: https://developer.gene.com/.well-known/openid-configuration
  sources:
  - well-known/genentech-openid-configuration.json
  type: openIdConnect
- endpoints:
    end_session: https://developer.gene.com/services/auth/idp/oidc/logout
    introspection: https://developer.gene.com/services/oauth2/introspect
    jwks_uri: https://developer.gene.com/id/keys
    registration: https://developer.gene.com/services/oauth2/register
    revocation: https://developer.gene.com/services/oauth2/revoke
    userinfo: https://developer.gene.com/services/oauth2/userinfo
  flows:
  - authorizationUrl: https://developer.gene.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://developer.gene.com/services/oauth2/token
  id_token_signing_alg:
  - RS256
  name: oauth2
  sources:
  - well-known/genentech-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
- description: Per-organization API keys provisioned via the Genentech Integration Marketplace, per the Universal API Implementation Guide.
  in: header
  name: apiKey
  sources:
  - https://fhir.developer.gene.com/
  type: apiKey
slug: genentech-authentication
source_filename: genentech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.gene.com/.well-known/openid-configuration\ndocs: https://developer.gene.com/s/api-library\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, implicit]\n  notes: >-\n    The Genentech Developer Portal / Integration Marketplace is fronted by a\n    Salesforce Experience Cloud identity provider exposing a full OpenID\n    Connect discovery document. FHIR UAPI connectivity is registration-based:\n    the Implementation Guide instructs partners to register through the\n    Integration Marketplace and provision API keys per organization, on top of\n    the OAuth2/OIDC authorization surface below.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://developer.gene.com/.well-known/openid-configuration\n  issuer: https://developer.gene.com\n  sources: [well-known/genentech-openid-configuration.json]\n- name: oauth2\n  type:\
  \ oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developer.gene.com/services/oauth2/authorize\n    tokenUrl: https://developer.gene.com/services/oauth2/token\n  endpoints:\n    userinfo: https://developer.gene.com/services/oauth2/userinfo\n    revocation: https://developer.gene.com/services/oauth2/revoke\n    introspection: https://developer.gene.com/services/oauth2/introspect\n    registration: https://developer.gene.com/services/oauth2/register\n    end_session: https://developer.gene.com/services/auth/idp/oidc/logout\n    jwks_uri: https://developer.gene.com/id/keys\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg: [RS256]\n  sources: [well-known/genentech-openid-configuration.json]\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-organization API keys provisioned via the Genentech Integration\n    Marketplace, per the Universal API Implementation Guide.\n  sources:\
  \ [https://fhir.developer.gene.com/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genentech/refs/heads/main/authentication/genentech-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Healthcare
- Life Sciences
- FHIR
- Patient Support Services
- Drug Discovery
- Genomics
---
