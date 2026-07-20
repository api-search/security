---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lingco Language Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lingco Language Labs secures its APIs with openIdConnect and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lingco Language Labs
provider_slug: lingco-language-labs
scheme_count: 7
schemes:
- domain: class.lingco.io
  initiation_url: https://class.lingco.io/api/lti1p3/login
  jwks_file: authentication/lingco-language-labs-lti1p3-jwks.json
  jwks_uri: https://class.lingco.io/api/lti1p3/keys
  key_algorithm: RS256
  name: lti-1p3-oidc
  platforms_documented:
  - docs: https://help.lingco.io/en/articles/10768792-lti-1-3-integration-in-canvas
    name: Canvas
  - docs: https://help.lingco.io/en/articles/11642193-lti-1-3-integration-in-schoology
    name: Schoology
  redirect_uri: https://class.lingco.io/api/lti1p3/launch
  registration:
    method: manual
    note: administrator sends the Client ID and Deployment ID to Lingco to complete setup
  role: Lingco is the tool; the LMS is the platform
  services_consumed:
  - id: ags
    name: Assignment and Grade Services
    note: line items, scores and results; consumed on every launch
  - id: nrps
    name: Names and Role Provisioning Services
    note: context membership; consumed on every launch
  standard: IMS/1EdTech LTI 1.3 (OIDC third-party-initiated login)
  target_link_uri: https://class.lingco.io/api/lti1p3/launch
  type: openIdConnect
- direction: outbound
  docs: https://help.lingco.io/en/articles/4379311-setting-up-canvas-api-integration
  flow: authorizationCode
  name: canvas-api-oauth2
  note: Lingco is the API client here, not the provider. The institution creates a Canvas developer key named "Lingco Classroom" and Lingco calls the Canvas REST API with it to sync grades and rosters beyond standard LTI.
  redirect_uri: https://class.lingco.io/auth/canvas/callback
  registration:
    method: manual
    note: administrator sends the App ID, Developer Key and Canvas URL domain to Lingco
  scope_surface:
    endpoint_groups:
    - assignment_groups
    - assignments
    - courses
    - external_tools
    - modules
    - sections
    - submissions
    - tabs
    - users_enrollments
    note: scopes are Canvas API scopes granted to Lingco, listed in the article when the institution enforces scope restrictions
  type: oauth2
- credentials:
  - Client Key + Client Secret (PowerSchool, ClassLink)
  - Client ID + Client Secret (Infinite Campus)
  direction: outbound
  docs: https://help.lingco.io/en/articles/11831372-oneroster-integration
  name: oneroster-client-credentials
  note: Lingco consumes the SIS OneRoster endpoint with a client key/secret issued by the district's SIS. Lingco does not host a OneRoster endpoint.
  standard: IMS/1EdTech OneRoster v1.1
  type: oauth2
- docs: https://help.lingco.io/en/articles/8733059-configuring-lingco-sso-with-google-and-google-classroom
  name: sso-google
  note: Lingco SSO with Google and Google Classroom
  type: openIdConnect
- docs: https://help.lingco.io/en/articles/15024126-lingco-sso-in-clever
  name: sso-clever
  note: Lingco SSO in Clever
  type: oauth2
- docs: https://help.lingco.io/en/articles/11201127-configuring-lingco-sso-in-schoology
  name: sso-schoology
  note: Lingco SSO in Schoology
  type: oauth2
- docs: https://help.lingco.io/en/articles/8519048-lti-single-sign-on-with-canvas-account-level-installation
  name: sso-canvas-lti-account-level
  note: LTI single sign on with Canvas, account-level installation
  type: openIdConnect
slug: lingco-language-labs-authentication
source_filename: lingco-language-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.lingco.io/en/collections/2522345-for-it-administrators\ndocs: https://help.lingco.io/en/articles/10768792-lti-1-3-integration-in-canvas\nnotes: >-\n  Lingco publishes no OpenAPI and no general-purpose developer API, so this\n  profile is not derived from securitySchemes. It captures the authentication\n  contracts Lingco actually documents for IT administrators: an LTI 1.3 tool\n  (OIDC third-party-initiated login), an OAuth2 authorization-code callback for\n  the Canvas API client, and OneRoster v1.1 client-credential rostering. There\n  is no self-service developer credential: Canvas and LTI registrations are\n  completed by sending the client/deployment identifiers to Lingco engineering.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  self_service: false\n  registration: manual, out-of-band with Lingco engineering\nschemes:\n- name: lti-1p3-oidc\n  type: openIdConnect\n  standard: IMS/1EdTech LTI 1.3 (OIDC\
  \ third-party-initiated login)\n  role: Lingco is the tool; the LMS is the platform\n  initiation_url: https://class.lingco.io/api/lti1p3/login\n  target_link_uri: https://class.lingco.io/api/lti1p3/launch\n  redirect_uri: https://class.lingco.io/api/lti1p3/launch\n  jwks_uri: https://class.lingco.io/api/lti1p3/keys\n  jwks_file: authentication/lingco-language-labs-lti1p3-jwks.json\n  key_algorithm: RS256\n  domain: class.lingco.io\n  services_consumed:\n  - id: ags\n    name: Assignment and Grade Services\n    note: line items, scores and results; consumed on every launch\n  - id: nrps\n    name: Names and Role Provisioning Services\n    note: context membership; consumed on every launch\n  registration:\n    method: manual\n    note: administrator sends the Client ID and Deployment ID to Lingco to complete\n      setup\n  platforms_documented:\n  - name: Canvas\n    docs: https://help.lingco.io/en/articles/10768792-lti-1-3-integration-in-canvas\n  - name: Schoology\n    docs: https://help.lingco.io/en/articles/11642193-lti-1-3-integration-in-schoology\n\
  - name: canvas-api-oauth2\n  type: oauth2\n  flow: authorizationCode\n  direction: outbound\n  note: >-\n    Lingco is the API client here, not the provider. The institution creates a\n    Canvas developer key named \"Lingco Classroom\" and Lingco calls the Canvas\n    REST API with it to sync grades and rosters beyond standard LTI.\n  redirect_uri: https://class.lingco.io/auth/canvas/callback\n  docs: https://help.lingco.io/en/articles/4379311-setting-up-canvas-api-integration\n  scope_surface:\n    note: scopes are Canvas API scopes granted to Lingco, listed in the article when\n      the institution enforces scope restrictions\n    endpoint_groups:\n    - assignment_groups\n    - assignments\n    - courses\n    - external_tools\n    - modules\n    - sections\n    - submissions\n    - tabs\n    - users_enrollments\n  registration:\n    method: manual\n    note: administrator sends the App ID, Developer Key and Canvas URL domain to Lingco\n- name: oneroster-client-credentials\n  type:\
  \ oauth2\n  standard: IMS/1EdTech OneRoster v1.1\n  direction: outbound\n  note: >-\n    Lingco consumes the SIS OneRoster endpoint with a client key/secret issued\n    by the district's SIS. Lingco does not host a OneRoster endpoint.\n  credentials:\n  - Client Key + Client Secret (PowerSchool, ClassLink)\n  - Client ID + Client Secret (Infinite Campus)\n  docs: https://help.lingco.io/en/articles/11831372-oneroster-integration\n- name: sso-google\n  type: openIdConnect\n  note: Lingco SSO with Google and Google Classroom\n  docs: https://help.lingco.io/en/articles/8733059-configuring-lingco-sso-with-google-and-google-classroom\n- name: sso-clever\n  type: oauth2\n  note: Lingco SSO in Clever\n  docs: https://help.lingco.io/en/articles/15024126-lingco-sso-in-clever\n- name: sso-schoology\n  type: oauth2\n  note: Lingco SSO in Schoology\n  docs: https://help.lingco.io/en/articles/11201127-configuring-lingco-sso-in-schoology\n- name: sso-canvas-lti-account-level\n  type: openIdConnect\n\
  \  note: LTI single sign on with Canvas, account-level installation\n  docs: https://help.lingco.io/en/articles/8519048-lti-single-sign-on-with-canvas-account-level-installation\nnot_found:\n- api keys / personal access tokens for a Lingco-hosted API\n- a public OAuth authorization server or /.well-known/openid-configuration on any\n  Lingco host\n- documented scope strings issued by Lingco\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingco-language-labs/refs/heads/main/authentication/lingco-language-labs-authentication.yml
summary_line: openIdConnect/oauth2 · 7 schemes
tags:
- Company
- Education
- EdTech
- Language Learning
- Learning Management
- LTI
- OneRoster
- Rostering
- Single Sign On
- Interoperability
---
