---
api_key_in: []
api_specs:
- filename: aerin-medical-discovery-api-openapi.yml
  format: yaml
  label: Aerin Medical Discovery API
  slug: aerin-medical-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-discovery-api-openapi.yml
- filename: aerin-medical-embed-api-openapi.yml
  format: yaml
  label: Aerin Medical Embed API
  slug: aerin-medical-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-embed-api-openapi.yml
- filename: aerin-medical-forms-api-openapi.yml
  format: yaml
  label: Aerin Medical Forms API
  slug: aerin-medical-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-forms-api-openapi.yml
- filename: aerin-medical-locator-api-openapi.yml
  format: yaml
  label: Aerin Medical Locator API
  slug: aerin-medical-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-locator-api-openapi.yml
- filename: aerin-medical-search-api-openapi.yml
  format: yaml
  label: Aerin Medical Search API
  slug: aerin-medical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/openapi/aerin-medical-search-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aerin Medical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aerin Medical secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aerin Medical
provider_slug: aerin-medical
scheme_count: 2
schemes:
- description: 'No credential required. All 15 catalogued operations — the doctor-finder collection, the locator widget, site search, oEmbed, the route-discovery documents, the footer, and the seven aerin-namespace form POSTs — accept unauthenticated requests. CORS is fully open (Access-Control-Allow-Origin: *), so browser callers on any origin can reach them.'
  evidence:
    fetched: '2026-07-31'
    observed: HTTP 200 on every catalogued read operation with no Authorization header.
  name: anonymous
  sources:
  - openapi/aerin-medical-site-openapi.yml
  type: none
- authorization_endpoint: https://aerinmedical.com/wp-admin/authorize-application.php
  description: WordPress application passwords, advertised by the site's own route index at authentication.application-passwords.endpoints.authorization. This is the built-in WordPress mechanism for authenticated calls and exists on every WordPress install; it is not an Aerin Medical developer programme.
  name: applicationPassword
  publicly_obtainable: false
  scheme: basic
  sources:
  - openapi/aerin-medical-site-openapi.yml
  - https://aerinmedical.com/wp-json/
  type: http
slug: aerin-medical-authentication
source_filename: aerin-medical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nprobe: true\nsource: openapi/aerin-medical-site-openapi.yml + live probes of https://aerinmedical.com/wp-json\ndocs: null\nsummary:\n  types: [none, http]\n  api_key_in: []\n  oauth2_flows: []\n  public_credential_available: false\n  anonymous_access: true\nmodel: >-\n  Aerin Medical has no developer authentication story: no sign-up, no API keys, no OAuth, no\n  OIDC, no scopes, no tokens, and no documented auth page. The only scheme the platform\n  advertises is WordPress application passwords, which are issued by the site's own\n  administrators and are not obtainable by the public. Every operation catalogued in openapi/\n  is reachable ANONYMOUSLY with no credential; the routes that are NOT reachable are blocked\n  outright at the edge rather than gated behind an obtainable credential.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    No credential required. All 15 catalogued operations — the doctor-finder collection,\
  \ the\n    locator widget, site search, oEmbed, the route-discovery documents, the footer, and the\n    seven aerin-namespace form POSTs — accept unauthenticated requests. CORS is fully open\n    (Access-Control-Allow-Origin: *), so browser callers on any origin can reach them.\n  sources: [openapi/aerin-medical-site-openapi.yml]\n  evidence:\n    fetched: '2026-07-31'\n    observed: HTTP 200 on every catalogued read operation with no Authorization header.\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, advertised by the site's own route index at\n    authentication.application-passwords.endpoints.authorization. This is the built-in\n    WordPress mechanism for authenticated calls and exists on every WordPress install; it is\n    not an Aerin Medical developer programme.\n  authorization_endpoint: https://aerinmedical.com/wp-admin/authorize-application.php\n  publicly_obtainable: false\n  sources: [openapi/aerin-medical-site-openapi.yml,\
  \ 'https://aerinmedical.com/wp-json/']\nrestricted_surface:\n  mechanism: iThemes Security plugin (route-level restriction)\n  status: 401\n  code: itsec_rest_api_access_restricted\n  affected:\n  - /wp/v2/posts\n  - /wp/v2/pages\n  - /wp/v2/media\n  - /wp/v2/categories\n  - /wp/v2/tags\n  - /wp/v2/users\n  - /wp/v2/comments\n  - /wp/v2/types\n  - /wp/v2/taxonomies\n  - /wp/v2/statuses\n  - /wp/v2/blocks\n  - /wp/v2/navigation\n  note: >-\n    Unusually for a WordPress site the content collections are closed while the company's own\n    custom plugin routes are wide open. The posture is inverted relative to data sensitivity:\n    the closed routes hold public marketing copy, while the open locator route returns\n    internal CRM fields — see security/aerin-medical-domain-security.yml, exposures[].\nnot_present:\n  oauth2: /.well-known/oauth-authorization-server returns 404 on every host\n  oidc: /.well-known/openid-configuration returns 404 on every host\n  api_keys: no key issuance, no\
  \ developer sign-up, no key header documented or observed\n  mtls: not offered\n  scopes: no scope surface exists, so scopes/ was deliberately not written\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerin-medical/refs/heads/main/authentication/aerin-medical-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Medical Devices
- Healthcare
- ENT
- Otolaryngology
- Rhinology
- Radiofrequency Ablation
- Nasal Airway Obstruction
- Chronic Rhinitis
- Physician Locator
- Private Company
---
