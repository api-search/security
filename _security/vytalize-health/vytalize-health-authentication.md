---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Vytalize Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vytalize Health secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vytalize Health
provider_slug: vytalize-health
scheme_count: 1
schemes:
- applies_to: https://app.vytalizehealth.com/
  authorization_endpoint: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/oauth2/v2.0/authorize
  client_library: '@azure/msal-browser (MSAL.js), bundled in the portal SPA'
  issuer: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0
  jwks_uri: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/discovery/v2.0/keys
  name: microsoft-entra-id
  openIdConnectUrl: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0/.well-known/openid-configuration
  provider: Microsoft Entra ID (Azure AD), single-tenant
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - https://app.vytalizehealth.com/static/js/main.2d65df30.js
  tenant_id: f44e254b-1755-4e18-b889-77701573aa22
  token_endpoint: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/oauth2/v2.0/token
  type: openIdConnect
slug: vytalize-health-authentication
source_filename: vytalize-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://app.vytalizehealth.com/static/js/main.2d65df30.js (partner portal bundle) and\n  https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0/.well-known/openid-configuration\nscope_of_this_record: >-\n  THIS IS NOT A DOCUMENTED API AUTHENTICATION PROFILE. Vytalize Health publishes no API reference and\n  no authentication documentation. What is recorded below is the identity layer of its partner web\n  portal, observed by reading the portal's own public JavaScript bundle and then fetching the\n  resulting (publicly served) OpenID Connect discovery document. It describes how a human practice\n  partner signs in to app.vytalizehealth.com, not how a machine client would authenticate to an API.\n  No `Authentication` pointer is wired into apis.yml for this file, because doing so would credit the\n  company with documented API authentication it does not publish.\nsummary:\n  types:\n  - openIdConnect\n\
  \  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  documented_by_provider: false\nschemes:\n- name: microsoft-entra-id\n  type: openIdConnect\n  openIdConnectUrl: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0/.well-known/openid-configuration\n  provider: Microsoft Entra ID (Azure AD), single-tenant\n  tenant_id: f44e254b-1755-4e18-b889-77701573aa22\n  issuer: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0\n  authorization_endpoint: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/oauth2/v2.0/authorize\n  token_endpoint: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/oauth2/v2.0/token\n  jwks_uri: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/discovery/v2.0/keys\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  client_library: '@azure/msal-browser (MSAL.js), bundled in the portal SPA'\n  applies_to: https://app.vytalizehealth.com/\n\
  \  sources:\n  - https://app.vytalizehealth.com/static/js/main.2d65df30.js\nx-evidence:\n- url: https://login.microsoftonline.com/f44e254b-1755-4e18-b889-77701573aa22/v2.0/.well-known/openid-configuration\n  status: 200\n  content_type: application/json\n- url: https://app.vytalizehealth.com/\n  status: 200\n  note: create-react-app shell titled \"Vytalize Health - Login\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vytalize-health/refs/heads/main/authentication/vytalize-health-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Healthcare
- Value Based Care
- Accountable Care Organization
- Medicare
- Population Health
- Clinical Decision Support
- Care Management
- Health Data
---
