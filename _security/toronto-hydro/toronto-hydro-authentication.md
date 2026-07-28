---
api_key_in: []
api_specs:
- filename: toronto-hydro-green-button-espi-openapi.yml
  format: yaml
  label: Toronto Hydro Green Button Connect My Data
  slug: toronto-hydro-green-button-connect-my-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-green-button-espi-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Toronto Hydro Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Toronto Hydro secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Toronto Hydro
provider_slug: toronto-hydro
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  sources:
  - openapi/toronto-hydro-green-button-espi-openapi.yml
  type: oauth2
slug: toronto-hydro-authentication
source_filename: toronto-hydro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/toronto-hydro-green-button-espi-openapi.yml\ndocs: https://www.torontohydro.com/documents/d/guest/green-button-connect-my-data-customer-guide\nnote: >-\n  The source specification is authored by the Green Button Alliance, not by Toronto Hydro,\n  and the authorizationUrl and tokenUrl below belong to the GBA sandbox. Toronto Hydro\n  publishes no OAuth endpoints, no scope reference and no anonymously served OpenID\n  Connect discovery document (see well-known/toronto-hydro-well-known.yml). What Toronto\n  Hydro does document, in its Green Button Connect My Data Customer Guide (PDF, 799 KB,\n  created 2024-10-21), is the customer-facing half of the flow, and it matches the\n  authorization-code model recorded here: the third party either emails the customer a\n  link or redirects them from its own app to \"Toronto Hydro's authentication page\", the\n  customer signs in with their Toronto Hydro online account (Option A)\
  \ or is offered \"an\n  alternative method to provide consent\" if they are not registered (Option B), and is\n  then redirected to the authorization page. Client credentials are issued only after the\n  third party is approved. The concrete Toronto Hydro endpoints were NOT observed and none\n  were invented.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  sources:\n  - openapi/toronto-hydro-green-button-espi-openapi.yml\nprovider_surface:\n  authentication_page_published: false\n  authentication_page_note: >-\n    Toronto Hydro names an authentication page in its Customer Guide\
  \ but does not publish\n    its URL. The two customer-facing management surfaces that ARE published both sit\n    behind the Liferay account login: https://www.torontohydro.com/my-account/green-button-data\n    (Download My Data) and https://www.torontohydro.com/my-account/green-button-connections\n    (manage and remove third-party Connect My Data connections).\n  token_endpoint_published: false\n  authorization_endpoint_published: false\n  oidc_discovery: false\n  credential_issuance: >-\n    After approval only — an online application through\n    https://torontoonboarding.savagedata.com/, a connectivity test, and acceptance of the\n    Third Party Terms and Conditions for Green Button Connect My Data.\n  consent_revocation: >-\n    The customer may revoke at any time and at their sole discretion, from the Green\n    Button connections page in their self-serve portal. Toronto Hydro's Third Party Terms\n    also state that Connect My Data is unavailable on or after the date a customer's\n\
  \    account is closed, including their final billing period.\ncross_links:\n  scopes: scopes/toronto-hydro-scopes.yml\n  conventions: conventions/toronto-hydro-conventions.yml\n  conformance: conformance/toronto-hydro-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/authentication/toronto-hydro-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Ontario
- Consumer Data
- Electricity Distribution
---
