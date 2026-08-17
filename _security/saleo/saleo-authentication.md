---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Saleo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Saleo secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Saleo
provider_slug: saleo
scheme_count: 3
schemes:
- applies_to: https://api.platform.saleo.io/scim/v2
  description: Long-lived API token minted in the Saleo Portal and pasted into the Okta provisioning "API Token" field. Saleo's documentation states the tokens "never expire, but can be revoked at any time" and can be deactivated if compromised or on routine rotation. There is no published expiry, refresh, or scope model — a token is org-wide for the SCIM surface.
  name: scimBearerToken
  rotation: manual revoke/deactivate, no expiry
  scheme: bearer
  scopes: none published
  sources:
  - https://help.saleo.io/articles/5029724323-how-to-configure-scim-within-saleo-s-okta-integration-network-app
  type: http
- applies_to: https://app.platform.saleo.io/
  description: SAML 2.0 single sign-on for human access to the Saleo Portal and the Saleo Chrome extension. Customers supply a SAML Sign-On URL, SAML Issuer and SAML Certificate from their identity provider. Okta ships a pre-built Saleo app; Okta also publishes a Saleo-specific SAML configuration guide.
  name: saml2SSO
  sources:
  - https://help.saleo.io/articles/2779294893-configuring-saml-based-sso-in-saleo
  - https://help.saleo.io/articles/9198269906-single-sign-on-sso-okta-setup-guide
  - https://saml-doc.okta.com/SAML_Docs/How-to-Configure-SAML-2.0-for-Saleo.html
  - https://www.okta.com/integrations/saleo/
  type: saml2
- applies_to: https://api.platform.saleo.io/v1/
  description: The RPC-style product API at https://api.platform.saleo.io/v1/* that backs the Saleo Portal, Chrome extension and tour viewer is customer-authenticated and entirely undocumented. Its own authentication entry points are visible in the first-party tour-viewer bundle (authenticate_by_email, authenticate_by_token, authenticate_by_provider, authenticate_by_tourlink, authenticate_by_viewer_token, authenticate_workato, create_scim_access_token) but Saleo publishes no reference for any of them. Unauthenticated calls return HTTP 401 {"message":"UNAUTHENTICATED"}.
  name: productApiSessionAuth
  published: false
  type: unpublished
slug: saleo-authentication
source_filename: saleo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.saleo.io/articles/5029724323-how-to-configure-scim-within-saleo-s-okta-integration-network-app\ndocs: https://help.saleo.io/collections/user-management-authentication\nnote: >-\n  Saleo publishes no OpenAPI, so nothing here is derived from a specification.\n  Every scheme below is taken from Saleo's own knowledge-base articles, the Okta\n  Integration Network listing for Saleo, or an unauthenticated HTTP probe of the\n  live endpoint recorded in x-evidence.\nsummary:\n  types: [http]\n  api_key_in: [header]\n  oauth2_flows: []\n  human_sso: [saml2]\nschemes:\n- name: scimBearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    Long-lived API token minted in the Saleo Portal and pasted into the Okta\n    provisioning \"API Token\" field. Saleo's documentation states the tokens\n    \"never expire, but can be revoked at any time\" and can be deactivated if\n    compromised or on routine rotation. There\
  \ is no published expiry, refresh, or\n    scope model — a token is org-wide for the SCIM surface.\n  applies_to: https://api.platform.saleo.io/scim/v2\n  rotation: manual revoke/deactivate, no expiry\n  scopes: none published\n  sources:\n  - https://help.saleo.io/articles/5029724323-how-to-configure-scim-within-saleo-s-okta-integration-network-app\n- name: saml2SSO\n  type: saml2\n  description: >-\n    SAML 2.0 single sign-on for human access to the Saleo Portal and the Saleo\n    Chrome extension. Customers supply a SAML Sign-On URL, SAML Issuer and SAML\n    Certificate from their identity provider. Okta ships a pre-built Saleo app;\n    Okta also publishes a Saleo-specific SAML configuration guide.\n  applies_to: https://app.platform.saleo.io/\n  sources:\n  - https://help.saleo.io/articles/2779294893-configuring-saml-based-sso-in-saleo\n  - https://help.saleo.io/articles/9198269906-single-sign-on-sso-okta-setup-guide\n  - https://saml-doc.okta.com/SAML_Docs/How-to-Configure-SAML-2.0-for-Saleo.html\n\
  \  - https://www.okta.com/integrations/saleo/\n- name: productApiSessionAuth\n  type: unpublished\n  description: >-\n    The RPC-style product API at https://api.platform.saleo.io/v1/* that backs the\n    Saleo Portal, Chrome extension and tour viewer is customer-authenticated and\n    entirely undocumented. Its own authentication entry points are visible in the\n    first-party tour-viewer bundle (authenticate_by_email, authenticate_by_token,\n    authenticate_by_provider, authenticate_by_tourlink, authenticate_by_viewer_token,\n    authenticate_workato, create_scim_access_token) but Saleo publishes no reference\n    for any of them. Unauthenticated calls return HTTP 401 {\"message\":\"UNAUTHENTICATED\"}.\n  applies_to: https://api.platform.saleo.io/v1/\n  published: false\noauth2: not offered\nopenid_connect: not offered\nmtls: not offered\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://api.platform.saleo.io/scim/v2/Users\n  http_status: 401\n  body: '{\"schemas\":[\"urn:ietf:params:scim:api:messages:2.0:Error\"\
  ],\"status\":\"401\",\"detail\":\"UNAUTHORIZED\"}'\n- fetched: '2026-08-13'\n  url: https://api.platform.saleo.io/scim/v2/ServiceProviderConfig\n  http_status: 401\n  note: >-\n    RFC 7644 section 4 permits ServiceProviderConfig, ResourceTypes and Schemas to be\n    served anonymously; Saleo gates all three, so the SCIM feature set cannot be read\n    without a customer token.\n- fetched: '2026-08-13'\n  url: https://api.platform.saleo.io/v1/authenticate_by_email\n  http_status: 401\n  body: '{\"message\":\"UNAUTHENTICATED\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saleo/refs/heads/main/authentication/saleo-authentication.yml
summary_line: http · 3 schemes
tags:
- Company
- Sales Tech
- Demo Automation
- Sales Enablement
- Presales
- Go-To-Market
- AI Agents
- SCIM
- Identity Provisioning
- Single Sign-On
- Interactive Demos
- Product Tours
---
