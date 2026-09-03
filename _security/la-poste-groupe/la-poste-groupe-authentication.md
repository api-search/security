---
api_key_in:
- cookie
- header
api_specs:
- filename: la-poste-groupe-suivi-openapi.json
  format: json
  label: La Poste Suivi v2
  slug: la-poste-suivi-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-suivi-openapi.json
- filename: la-poste-groupe-digiposte-openapi.json
  format: json
  label: Digiposte v3
  slug: digiposte-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-digiposte-openapi.json
- filename: la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
  format: json
  label: Lettre recommandee en ligne v1
  slug: lettre-recommandee-en-ligne-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
- filename: la-poste-groupe-open-data-openapi.json
  format: json
  label: La Poste Open Data v1
  slug: la-poste-open-data-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/openapi/la-poste-groupe-open-data-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: La Poste Groupe Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: La Poste Groupe secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: La Poste Groupe
provider_slug: la-poste-groupe
scheme_count: 7
schemes:
- name: basic
  scheme: basic
  sources:
  - openapi/la-poste-groupe-digiposte-openapi.json
  type: http
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    scopes: 0
    tokenUrl: /
  name: oauth2
  sources:
  - openapi/la-poste-groupe-digiposte-openapi.json
  type: oauth2
- flows:
  - authorizationUrl: https://test.com
    flow: implicit
    scopes: 0
  name: default
  sources:
  - openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json
  type: oauth2
- in: header
  name: apiKey
  parameter: x-apiKey
  sources:
  - openapi/la-poste-groupe-open-data-openapi.json
  type: apiKey
- in: cookie
  name: sdCookie
  parameter: id_token
  sources:
  - openapi/la-poste-groupe-open-data-openapi.json
  type: apiKey
- in: header
  name: OKAPIkey
  parameter: X-Okapi-Key
  sources:
  - openapi/la-poste-groupe-suivi-openapi.json
  type: apiKey
- in: cookie
  name: JWT
  parameter: access_token
  sources:
  - openapi/la-poste-groupe-suivi-openapi.json
  type: apiKey
slug: la-poste-groupe-authentication
source_filename: la-poste-groupe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/la-poste-groupe-digiposte-openapi.json, openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json,\n  openapi/la-poste-groupe-open-data-openapi.json, openapi/la-poste-groupe-suivi-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/la-poste-groupe-digiposte-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    tokenUrl: /\n    scopes: 0\n  sources:\n  - openapi/la-poste-groupe-digiposte-openapi.json\n- name: default\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://test.com\n    scopes: 0\n  sources:\n  - openapi/la-poste-groupe-lettre-recommandee-en-ligne-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-apiKey\n\
  \  sources:\n  - openapi/la-poste-groupe-open-data-openapi.json\n- name: sdCookie\n  type: apiKey\n  in: cookie\n  parameter: id_token\n  sources:\n  - openapi/la-poste-groupe-open-data-openapi.json\n- name: OKAPIkey\n  type: apiKey\n  in: header\n  parameter: X-Okapi-Key\n  sources:\n  - openapi/la-poste-groupe-suivi-openapi.json\n- name: JWT\n  type: apiKey\n  in: cookie\n  parameter: access_token\n  sources:\n  - openapi/la-poste-groupe-suivi-openapi.json\ndocs: https://developer.laposte.fr/getting-started\nprimary_model: >-\n  API key in the X-Okapi-Key request header, issued per application on\n  developer.laposte.fr and bound to a plan subscription. Confirmed live: an\n  unauthenticated GET of https://api.laposte.fr/suivi/v2/idships/6M20132968235 on\n  2026-09-02 returned HTTP 401 with\n  {\"code\":\"UNAUTHORIZED\",\"message\":\"This action requires an authorization\"}.\nsandbox_keys: >-\n  The same header carries both production and sandbox keys; nothing in the\n  credential distinguishes\
  \ the two. See sandbox/la-poste-groupe-sandbox.yml.\nplaceholder_warnings:\n- scheme: oauth2 (Digiposte v3)\n  finding: >-\n    authorizationUrl and tokenUrl are both the literal \"/\". The real token endpoint\n    is POST /digiposte/v3/oauth/token, discoverable only from the path list. Basic\n    auth mints the client_credentials token; bearer is used thereafter.\n- scheme: default (Lettre recommandee en ligne v1)\n  finding: >-\n    authorizationUrl is https://test.com - a springdoc generator default that\n    reached production. Not a usable authorization server; treat this API's\n    credential model as undocumented.\n- scheme: JWT (Suivi v2)\n  finding: >-\n    Declared as an apiKey in an access_token COOKIE. This is the browser-session\n    path, not a server-to-server one; server integrations use X-Okapi-Key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-poste-groupe/refs/heads/main/authentication/la-poste-groupe-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Company
- Logistics
- Shipping
- Package Tracking
- Postal
- Addresses
- Geocoding
- Open Data
- Document Management
- Identity
- Government
- France
---
