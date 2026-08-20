---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Casavo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Casavo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Casavo
provider_slug: casavo
scheme_count: 3
schemes:
- description: Casavo's help-centre article "Documentazione API" told integrators they would receive an invitation to a sandbox area from which they could retrieve their API keys to test before moving to production. The header/parameter name is not published anywhere public; the API exposes an `apikey` collection (https://editor.realisti.co/api/v4/apikey/) which itself requires authentication, so key management is self-service only for existing customers.
  evidence:
    apikey_collection: https://editor.realisti.co/api/v4/apikey/
    apikey_collection_status: 401
    archived_copy: https://web.archive.org/web/20210922202055/https://help.casavo.com/documentazione-api
    documented_by: https://help.casavo.com/documentazione-api
    documented_by_status: 404
  id: api_key
  in: unknown
  name: unknown
  status: documented
  type: apiKey
- description: The API host is a Django/DRF application fronted by uvicorn. The API index sets a `csrftoken` cookie and the responses `Vary` on `Authorization` and `Cookie`, indicating both a session/cookie path (used by the editor.realisti.co web application at /login/) and an Authorization-header path.
  evidence:
    login_page: https://editor.realisti.co/login/
    login_page_status: 200
    probe: https://editor.realisti.co/api/v4/
    probe_status: 200
    set_cookie: csrftoken
    vary_header: Origin, Accept-Language, Authorization, Cookie
  id: session
  status: observed
  type: http
- description: A dedicated `auth` collection is advertised in the v4 and v2 API indexes. It answers 401 anonymously, so the grant shape (token exchange vs. login) cannot be read without credentials.
  evidence:
    probe_status: 401
  id: auth_endpoint
  status: observed
  type: endpoint
  url: https://editor.realisti.co/api/v4/auth/
slug: casavo-authentication
source_filename: casavo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://editor.realisti.co/api/v4/\nname: Casavo Virtual Tools (Realisti.co) API — authentication profile\napi: casavo:virtual-tools\nsummary: >-\n  No OpenAPI is published for the Realisti.co API, so this profile is built from live anonymous\n  probes of the API host plus Casavo's own (now archived) help-centre integration article. Every\n  resource collection under /api/v4/ answers 401 with a DRF-style `not_authenticated` envelope;\n  only the collection index itself is anonymous. Casavo documents API-key issuance through an\n  invitation-only sandbox area, with the key then used against production.\nschemes:\n- id: api_key\n  type: apiKey\n  status: documented\n  in: unknown\n  name: unknown\n  description: >-\n    Casavo's help-centre article \"Documentazione API\" told integrators they would receive an\n    invitation to a sandbox area from which they could retrieve their API keys to test before\n    moving to production.\
  \ The header/parameter name is not published anywhere public; the API\n    exposes an `apikey` collection (https://editor.realisti.co/api/v4/apikey/) which itself\n    requires authentication, so key management is self-service only for existing customers.\n  evidence:\n    documented_by: https://help.casavo.com/documentazione-api\n    documented_by_status: 404\n    archived_copy: https://web.archive.org/web/20210922202055/https://help.casavo.com/documentazione-api\n    apikey_collection: https://editor.realisti.co/api/v4/apikey/\n    apikey_collection_status: 401\n- id: session\n  type: http\n  status: observed\n  description: >-\n    The API host is a Django/DRF application fronted by uvicorn. The API index sets a `csrftoken`\n    cookie and the responses `Vary` on `Authorization` and `Cookie`, indicating both a session/cookie\n    path (used by the editor.realisti.co web application at /login/) and an Authorization-header path.\n  evidence:\n    probe: https://editor.realisti.co/api/v4/\n\
  \    probe_status: 200\n    vary_header: 'Origin, Accept-Language, Authorization, Cookie'\n    set_cookie: csrftoken\n    login_page: https://editor.realisti.co/login/\n    login_page_status: 200\n- id: auth_endpoint\n  type: endpoint\n  status: observed\n  url: https://editor.realisti.co/api/v4/auth/\n  description: >-\n    A dedicated `auth` collection is advertised in the v4 and v2 API indexes. It answers 401\n    anonymously, so the grant shape (token exchange vs. login) cannot be read without credentials.\n  evidence:\n    probe_status: 401\noauth2: false\nopenid_connect: false\nmutual_tls: false\nanonymous_surface:\n- url: https://editor.realisti.co/api/v4/\n  status: 200\n  note: Collection index — 28 resource links, no auth required.\n- url: https://editor.realisti.co/api/v3/\n  status: 200\n  note: Legacy index — view, viewdraft.\n- url: https://editor.realisti.co/api/v2/\n  status: 200\n  note: Legacy index — house, housedraft, floordraft, viewdraft, targetdraft, auth.\n- url:\
  \ https://editor.realisti.co/api/v4/agency/fe27904b8bee4cb2a922c0f2092b5f0e/?levels=2&customizations\n  status: 200\n  note: >-\n    Agency detail is readable anonymously by object id — this is the read path the embedded\n    virtual-tour viewer uses. It returns agency name, legal entity (ragione sociale), branding\n    profile and plan entitlement flags.\ngated_surface:\n- url: https://editor.realisti.co/api/v4/house/\n  status: 401\n- url: https://editor.realisti.co/api/v4/apikey/\n  status: 401\n- url: https://editor.realisti.co/api/v4/auth/\n  status: 401\ndocs: null\ndocs_note: >-\n  The only integration documentation Casavo published (help.casavo.com/documentazione-api and its\n  Spanish twin) is gone — the whole HubSpot-hosted help centre now returns 404 — and the API\n  reference it pointed at (https://editor.realisti.co/api/v4/docs/) also returns 404.\ngaps:\n- No OpenAPI, Swagger or GraphQL SDL published for the API.\n- API key transport (header name / query parameter) is not\
  \ documented publicly.\n- No OAuth 2.0 or OpenID Connect surface; no /.well-known/oauth-authorization-server.\n- The published API reference URL is dead, so no anonymous reader can learn the request shapes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casavo/refs/heads/main/authentication/casavo-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Real-Estate
- PropTech
- Marketplace
- Virtual Tours
- Property Listings
- Italy
- Spain
- France
- Mortgages
---
