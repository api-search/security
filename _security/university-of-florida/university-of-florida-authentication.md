---
api_key_in: []
api_specs:
- filename: university-of-florida-schedule-of-courses-openapi.yml
  format: yaml
  label: UF Schedule of Courses (SOC) API
  slug: soc-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-florida/refs/heads/main/openapi/university-of-florida-schedule-of-courses-openapi.yml
- filename: university-of-florida-libraries-patron-api-openapi.yml
  format: yaml
  label: UF Libraries Patron API
  slug: libraries-patron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-florida/refs/heads/main/openapi/university-of-florida-libraries-patron-api-openapi.yml
auth_types: []
description: 'Both institution-operated University of Florida APIs are entirely unauthenticated. No API key is issued, no registration exists, no developer portal exists, and no Authorization, WWW-Authenticate or rate-limit header appears on any response. This is not "auth is undocumented" — it is "there is no auth", verified by successfully reading real data with no credential of any kind.

  That has a consequence worth stating plainly: an agent can consume both APIs today with zero onboarding, and UF has no mechanism to identify, throttle or revoke any consumer.'
kind: authentication
layout: security
method: probed
name: University Of Florida Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Florida declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Florida
provider_slug: university-of-florida
scheme_count: 0
schemes: []
slug: university-of-florida-authentication
source_filename: university-of-florida-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: University of Florida\nproviderId: university-of-florida\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live unauthenticated requests to https://one.ufl.edu/apix/soc/schedule/,\n  https://one.ufl.edu/apix/soc/filters/ and every resource under\n  https://api.patron.uflib.ufl.edu on 2026-09-01, sent with no Authorization header, no\n  cookie and no API key, plus inspection of every response header returned.\ndescription: >-\n  Both institution-operated University of Florida APIs are entirely unauthenticated. No\n  API key is issued, no registration exists, no developer portal exists, and no\n  Authorization, WWW-Authenticate or rate-limit header appears on any response. This is\n  not \"auth is undocumented\" — it is \"there is no auth\", verified by successfully reading\n  real data with no credential of any kind.\n\n  That has a consequence worth stating plainly: an agent can consume\
  \ both APIs today with\n  zero onboarding, and UF has no mechanism to identify, throttle or revoke any consumer.\n\napis:\n- name: UF Schedule of Courses (SOC) API\n  baseURL: https://one.ufl.edu/apix/soc\n  x-operator: institution\n  authentication:\n    required: false\n    type: none\n    verified:\n      url: https://one.ufl.edu/apix/soc/schedule/?term=2268&last-control-number=0\n      status: 200\n      sent_credentials: none\n      note: 'Returned 4,624 Fall 2026 course rows with no credential.'\n  registration:\n    required: false\n    portal: none\n    note: 'No developer portal, no key issuance, no application process discovered.'\n  authorization:\n    scopes: none\n    note: 'No scope, tier or entitlement model. Every consumer sees the same public data.'\n\n- name: UF Libraries Patron API\n  baseURL: https://api.patron.uflib.ufl.edu\n  x-operator: institution\n  authentication:\n    required: false\n    type: none\n    verified:\n      url: https://api.patron.uflib.ufl.edu/types\n\
  \      status: 200\n      sent_credentials: none\n  registration:\n    required: false\n    portal: none\n  authorization:\n    scopes: none\n    note: >-\n      Records carry an `ip_restriction_mask` field, so the corpus DOES model\n      access restriction per item — but enforcement is by caller IP, not by any credential\n      the consumer presents. There is no way for a consumer to authenticate in order to\n      widen access.\n\ninstitutional_authentication:\n  note: >-\n    UF's enterprise authentication is GatorLink, fronted by a self-hosted Shibboleth\n    Identity Provider at https://login.ufl.edu/idp/shibboleth, registered in InCommon and\n    interfederated into eduGAIN. It is SAML 2.0 and SAML 1.1, and it is the authentication\n    surface for UF's gated systems — including data.ufl.edu, which redirects an\n    unauthenticated caller straight to the Web Login Service. It is NOT an API\n    authentication mechanism for either public API above, and it does not issue tokens to\n\
  \    third-party developers. Documented in identity-federation/.\n  entityID: https://login.ufl.edu/idp/shibboleth\n  protocols: [SAML 2.0, SAML 1.1, Shibboleth 1.0]\n  x-operator: institution\n\ngaps:\n- 'No OAuth 2.0, OIDC or API-key surface is published for either public API.'\n- 'No .well-known/oauth-protected-resource, no RFC 9728 metadata, no dynamic client registration.'\n- 'No terms of use, acceptable-use policy or attribution requirement is published for either API.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-florida/refs/heads/main/authentication/university-of-florida-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Florida
- Association of American Universities
- Course Catalog
- Digital Collections
- Library
- Research Data
- Identity Federation
- OAI-PMH
- Research Computing
---
