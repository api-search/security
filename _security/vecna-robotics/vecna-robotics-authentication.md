---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Vecna Robotics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Vecna Robotics secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Vecna Robotics
provider_slug: vecna-robotics
scheme_count: 1
schemes:
- claims_supported:
  - active
  - address
  - email
  - email_verified
  - family_name
  - given_name
  - is_app_installed
  - language
  - locale
  - name
  - nickname
  - organization_id
  - phone_number
  - phone_number_verified
  - photos
  - picture
  - preferred_username
  - profile
  - sub
  - updated_at
  - urls
  - user_id
  - user_type
  - zoneinfo
  dynamic_client_registration: true
  endpoints:
    authorization: https://vecnarobotics.my.site.com/services/oauth2/authorize
    end_session: https://vecnarobotics.my.site.com/services/auth/idp/oidc/logout
    introspection: https://vecnarobotics.my.site.com/services/oauth2/introspect
    jwks: https://vecnarobotics.my.site.com/id/keys
    registration: https://vecnarobotics.my.site.com/services/oauth2/register
    revocation: https://vecnarobotics.my.site.com/services/oauth2/revoke
    token: https://vecnarobotics.my.site.com/services/oauth2/token
    userinfo: https://vecnarobotics.my.site.com/services/oauth2/userinfo
  frontchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://vecnarobotics.my.site.com
  name: PartnerPortalOIDC
  openIdConnectUrl: https://vecnarobotics.my.site.com/.well-known/openid-configuration
  response_types_supported:
  - code
  - token
  - token id_token
  sources:
  - well-known/vecna-robotics-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  token_introspection: true
  type: openIdConnect
slug: vecna-robotics-authentication
source_filename: vecna-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://vecnarobotics.my.site.com/.well-known/openid-configuration\nnote: >-\n  Derived from the live, anonymously-served OpenID Connect discovery document on the\n  Vecna Robotics Salesforce Experience Cloud partner portal. Vecna Robotics publishes\n  no OpenAPI, so no securityScheme could be derived from a spec; this is the only\n  documented authentication surface in the estate. It authenticates partner-portal\n  users and portal-scoped platform API access — it is NOT a Vecna Robotics product\n  API credential.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: PartnerPortalOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://vecnarobotics.my.site.com/.well-known/openid-configuration\n  issuer: https://vecnarobotics.my.site.com\n  sources:\n  - well-known/vecna-robotics-openid-configuration.json\n  endpoints:\n    authorization:\
  \ https://vecnarobotics.my.site.com/services/oauth2/authorize\n    token: https://vecnarobotics.my.site.com/services/oauth2/token\n    userinfo: https://vecnarobotics.my.site.com/services/oauth2/userinfo\n    revocation: https://vecnarobotics.my.site.com/services/oauth2/revoke\n    introspection: https://vecnarobotics.my.site.com/services/oauth2/introspect\n    registration: https://vecnarobotics.my.site.com/services/oauth2/register\n    jwks: https://vecnarobotics.my.site.com/id/keys\n    end_session: https://vecnarobotics.my.site.com/services/auth/idp/oidc/logout\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  subject_types_supported:\n  - public\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  dynamic_client_registration: true\n  token_introspection: true\n  frontchannel_logout_supported: true\n  claims_supported:\n  - active\n  - address\n\
  \  - email\n  - email_verified\n  - family_name\n  - given_name\n  - is_app_installed\n  - language\n  - locale\n  - name\n  - nickname\n  - organization_id\n  - phone_number\n  - phone_number_verified\n  - photos\n  - picture\n  - preferred_username\n  - profile\n  - sub\n  - updated_at\n  - urls\n  - user_id\n  - user_type\n  - zoneinfo\ngaps:\n- No public product API, so no product-level authentication documentation exists.\n- No /.well-known/oauth-authorization-server (RFC 8414) or /.well-known/oauth-protected-resource\n  document published on any host.\n- Vecna markets \"flexible API integrations\" with WMS/MES/ERP but documents no auth\n  model for them publicly; integration credentials appear to be issued per deployment.\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://vecnarobotics.my.site.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vecna-robotics/refs/heads/main/authentication/vecna-robotics-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Robotics
- Warehouse Automation
- Autonomous Mobile Robots
- Material Handling
- Logistics
- Supply Chain
- Manufacturing
- Industrial Automation
- Robotics as a Service
---
