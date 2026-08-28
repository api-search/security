---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sidechef Authentication
name_suffix: Authentication
oauth_flows: []
overview: SideChef declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SideChef
provider_slug: sidechef
scheme_count: 2
schemes:
- description: Partner authentication identifier placed as a data attribute on the widget mount element. Because it ships in page markup it is a public partner identifier, not a secret credential.
  docs: https://business.sidechef.com/sb-documentation
  documented: true
  id: partnerKey
  in: html-attribute
  name: data-partner-key
  required: true
  rotation: not documented
  scopes: none
  surface: Shoppable Button component
  type: apiKey
- description: The widget bundle constructs an Authorization header of the form "Basic <credential>" for its API calls. SideChef publishes no documentation for this scheme; it is recorded here as observed behaviour of a publicly served script, not as a documented contract.
  documented: false
  evidence: 'The v2 widget bundle contains a fetch whose headers object sets Authorization: "Basic " + <credential> alongside Content-Type: application/json; charset=UTF-8.'
  id: httpBasic
  required: true
  rotation: not documented
  scheme: basic
  scopes: none
  surface: SideChef Widget API (v3)
  type: http
slug: sidechef-authentication
source_filename: sidechef-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  https://business.sidechef.com/sb-documentation plus live unauthenticated probes of\n  https://www.sidechef.com/v3/widget/recipes/ and inspection of the publicly served widget\n  bundle at https://www.scgrocery.net/widget/v2/\nnote: >-\n  Derived from probe evidence rather than from a securityScheme block: SideChef publishes\n  no OpenAPI and no authentication reference page. Nothing here is inferred beyond what a\n  public request or the publicly served JavaScript bundle demonstrates.\ndocs: https://business.sidechef.com/sb-documentation\nsummary: >-\n  Access is partner-scoped and issued by SideChef through a sales conversation. There is no\n  self-service signup, no developer portal, no key-management console, and no OAuth. The\n  partner identifier is carried in markup for the embedded component, and the REST surface\n  behind it uses HTTP Basic.\nschemes:\n- id: partnerKey\n  type: apiKey\n  in: html-attribute\n  name:\
  \ data-partner-key\n  surface: Shoppable Button component\n  required: true\n  documented: true\n  docs: https://business.sidechef.com/sb-documentation\n  description: >-\n    Partner authentication identifier placed as a data attribute on the widget mount\n    element. Because it ships in page markup it is a public partner identifier, not a\n    secret credential.\n  rotation: not documented\n  scopes: none\n- id: httpBasic\n  type: http\n  scheme: basic\n  surface: SideChef Widget API (v3)\n  required: true\n  documented: false\n  description: >-\n    The widget bundle constructs an Authorization header of the form \"Basic <credential>\"\n    for its API calls. SideChef publishes no documentation for this scheme; it is recorded\n    here as observed behaviour of a publicly served script, not as a documented contract.\n  evidence: >-\n    The v2 widget bundle contains a fetch whose headers object sets\n    Authorization: \"Basic \" + <credential> alongside\n    Content-Type: application/json;\
  \ charset=UTF-8.\n  rotation: not documented\n  scopes: none\noauth2: false\nopenid_connect: false\nmutual_tls: false\nunauthenticated_behaviour:\n  status: 401\n  content_type: application/json\n  body: '{\"status_code\":401,\"error\":\"Authentication credentials were not provided.\"}'\n  www_authenticate_header: not returned\n  note: >-\n    The message is the Django REST Framework default, indicating the v3 surface is a DRF\n    application. No WWW-Authenticate challenge is emitted, so an agent cannot discover the\n    scheme from the response alone.\naccess:\n  self_service: false\n  signup_url: none\n  process: contact sales via https://www.sidechef.com/business/contact-us\n  gate: sales-gate\nevidence:\n- url: https://www.sidechef.com/v3/widget/recipes/\n  status: 401\n  content_type: application/json\n- url: https://www.scgrocery.net/v3/widget/recipes/\n  status: 401\n  content_type: application/json\n- url: https://www.scgrocery.net/v3/widget/events/\n  status: 401\n  content_type:\
  \ application/json\n- url: https://www.scgrocery.net/widget/v2/\n  status: 200\n  content_type: application/javascript\n- url: https://business.sidechef.com/sb-documentation\n  status: 200\n- url: https://www.sidechef.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.sidechef.com/.well-known/oauth-authorization-server\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidechef/refs/heads/main/authentication/sidechef-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Food
- Recipes
- Retail
- Grocery
- Commerce
- Advertising
- Content
- Widgets
- Artificial Intelligence
- Nutrition
- Media
---
