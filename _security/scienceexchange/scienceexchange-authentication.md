---
api_key_in:
- query
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Scienceexchange Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Science Exchange secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Science Exchange
provider_slug: scienceexchange
scheme_count: 3
schemes:
- authorization_endpoint: https://app.scienceexchange.com/services/oauth2/authorize
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://app.scienceexchange.com/services/oauth2/introspect
  issuer: https://app.scienceexchange.com
  jwks_uri: https://app.scienceexchange.com/id/keys
  name: OpenIDConnect
  scheme: oidc
  sources:
  - well-known/scienceexchange-openid-configuration.json
  surface: app.scienceexchange.com login (Salesforce Experience Cloud / Identity)
  token_endpoint: https://app.scienceexchange.com/services/oauth2/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://app.scienceexchange.com/services/oauth2/userinfo
- name: EnterpriseSSO
  notes: SAML-based single sign-on, documented on /platform/integrations.
  providers:
  - Okta
  - Azure AD (Entra ID)
  sources:
  - https://www.scienceexchange.com/platform/integrations
  surface: platform login for enterprise customers
  type: saml
- in: query
  name: ProvidersApiKey
  notes: The first-party se_providers_api_client Ruby gem authenticates by appending the API key to each request as an access_token query parameter (lib/se_providers_api_client/client.rb).
  parameter: access_token
  sources:
  - https://github.com/scienceexchange/se_providers_api_client
  - https://demo.scienceexchange.com/api-docs/providers
  surface: Science Exchange Providers API
  type: apiKey
slug: scienceexchange-authentication
source_filename: scienceexchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://app.scienceexchange.com/.well-known/openid-configuration +\n  github.com/scienceexchange/se_providers_api_client (first-party gem source)\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - apiKey\n  oauth2_flows:\n  - authorizationCode\n  api_key_in:\n  - query\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  scheme: oidc\n  surface: app.scienceexchange.com login (Salesforce Experience Cloud / Identity)\n  issuer: https://app.scienceexchange.com\n  authorization_endpoint: https://app.scienceexchange.com/services/oauth2/authorize\n  token_endpoint: https://app.scienceexchange.com/services/oauth2/token\n  userinfo_endpoint: https://app.scienceexchange.com/services/oauth2/userinfo\n  introspection_endpoint: https://app.scienceexchange.com/services/oauth2/introspect\n  jwks_uri: https://app.scienceexchange.com/id/keys\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  sources:\n  - well-known/scienceexchange-openid-configuration.json\n- name: EnterpriseSSO\n  type: saml\n  surface: platform login for enterprise customers\n  providers:\n  - Okta\n  - Azure AD (Entra ID)\n  notes: SAML-based single sign-on, documented on /platform/integrations.\n  sources:\n  - https://www.scienceexchange.com/platform/integrations\n- name: ProvidersApiKey\n  type: apiKey\n  in: query\n  parameter: access_token\n  surface: Science Exchange Providers API\n  notes: >-\n    The first-party se_providers_api_client Ruby gem authenticates by\n    appending the API key to each request as an access_token query\n    parameter (lib/se_providers_api_client/client.rb).\n  sources:\n  - https://github.com/scienceexchange/se_providers_api_client\n  - https://demo.scienceexchange.com/api-docs/providers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scienceexchange/refs/heads/main/authentication/scienceexchange-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Life Sciences
- Research and Development
- Procurement
- Supplier Management
- Marketplace
- Biotech
- Pharmaceutical
- Scientific Research
---
