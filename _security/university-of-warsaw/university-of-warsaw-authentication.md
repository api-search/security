---
api_key_in:
- query
- header
api_specs:
- filename: university-of-warsaw-apiref-api-openapi.yml
  format: yaml
  label: University of Warsaw apiref API
  slug: university-of-warsaw-apiref-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-apiref-api-openapi.yml
- filename: university-of-warsaw-apisrv-api-openapi.yml
  format: yaml
  label: University of Warsaw apisrv API
  slug: university-of-warsaw-apisrv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-apisrv-api-openapi.yml
- filename: university-of-warsaw-calendar-api-openapi.yml
  format: yaml
  label: University of Warsaw calendar API
  slug: university-of-warsaw-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-calendar-api-openapi.yml
- filename: university-of-warsaw-courses-api-openapi.yml
  format: yaml
  label: University of Warsaw courses API
  slug: university-of-warsaw-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-courses-api-openapi.yml
- filename: university-of-warsaw-fac-api-openapi.yml
  format: yaml
  label: University of Warsaw fac API
  slug: university-of-warsaw-fac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-fac-api-openapi.yml
- filename: university-of-warsaw-jaskier-api-openapi.yml
  format: yaml
  label: Jaskier API
  slug: jaskier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-jaskier-api-openapi.yml
- filename: university-of-warsaw-sp4eu-api-openapi.yml
  format: yaml
  label: Student Portal 4EU+ API
  slug: sp4eu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-sp4eu-api-openapi.yml
auth_types:
- apiKey
- oauth1a
- bearer
- saml
description: ''
kind: authentication
layout: security
method: derived
name: University Of Warsaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Warsaw secures its APIs with apiKey, oauth1a, bearer, and saml across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Warsaw
provider_slug: university-of-warsaw
scheme_count: 4
schemes:
- api: university-of-warsaw:university-of-warsaw-apiref-api
  description: The USOS API uses OAuth 1.0a for authorized methods. A Consumer Key/Secret is obtained from the USOS developers portal (https://usosapps.uw.edu.pl/developers/ — the page renders the real registration form but answers HTTP 403 to non-browser clients), and an access token is obtained via the flow documented at https://usosapps.uw.edu.pl/developers/api/authorization/ (200). Anonymous methods such as services/apisrv/now and services/apiref/method_index need none of it.
  in: query
  name: oauth1a
  parameter: oauth_token
  sources:
  - openapi/_original/university-of-warsaw-usos-api.yaml
  - https://usosapps.uw.edu.pl/developers/api/authorization/
  type: apiKey
- api: university-of-warsaw:sp4eu-api
  description: 'The Student Portal 4EU+ API declares a single securityScheme, "Authorization" (apiKey, in header). Its 401 body is the only public documentation of the flow: "Please use /access/login endpoint to receive bearer token. Api key should be provided as header: Authorization: Bearer $BEARER_VALUE". Read endpoints such as GET /api/v1/Tutorial answer without it; the Admin subtree additionally role-gates and returns 403 "Access Denied".'
  in: header
  name: bearer
  parameter: Authorization
  sources:
  - openapi/_original/university-of-warsaw-sp4eu-api.json
  - https://api.sp4eu.uw.edu.pl/principal
  type: apiKey
- api: university-of-warsaw:jaskier-api
  description: Jaskier declares the same single "Authorization" apiKey header scheme. Every data endpoint probed anonymously returned 401; only /v3/api-docs and /api/v1/system/build are open. No public token-issuance path was found — the audience is the university's own applications.
  in: header
  name: bearer
  parameter: Authorization
  sources:
  - openapi/_original/university-of-warsaw-jaskier-api.json
  type: apiKey
- api: university-of-warsaw:saml-idp
  description: End-user authentication for the portals is federated SAML 2.0 against the university's own Shibboleth IdP, entityID https://login.uw.edu.pl/idp (metadata served at that URL, shibmd:Scope login.uw.edu.pl), fronted by an Apereo CAS login at logowanie.uw.edu.pl and registered in eduGAIN by PIONIER.Id. The Student Portal 4EU+ ships its own SP metadata at https://api.sp4eu.uw.edu.pl/saml2/service-provider-metadata and exposes /principal/edugain.
  in: browser
  name: saml
  parameter: SAMLResponse
  sources:
  - https://login.uw.edu.pl/idp
  - https://api.sp4eu.uw.edu.pl/saml2/service-provider-metadata
  type: federated
slug: university-of-warsaw-authentication
source_filename: university-of-warsaw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nx-evidence-method: probed  # schemes confirmed against live 401/403 responses and IdP metadata\nsource: >-\n  openapi/_original/university-of-warsaw-usos-api.yaml,\n  openapi/_original/university-of-warsaw-sp4eu-api.json,\n  openapi/_original/university-of-warsaw-jaskier-api.json, plus live probes of\n  https://api.sp4eu.uw.edu.pl, https://api.jaskier.uw.edu.pl and https://login.uw.edu.pl on\n  2026-09-01.\nx-operator: institution\nsummary:\n  types:\n  - apiKey\n  - oauth1a\n  - bearer\n  - saml\n  api_key_in:\n  - query\n  - header\nnote: >-\n  Three separate authentication regimes run under one institution. USOS uses OAuth 1.0a with a\n  Consumer Key/Secret issued by hand from the developers portal. The two springdoc services use a\n  bearer token in an Authorization header, obtained from /access/login, behind which sits the\n  university's own SAML identity provider. There is no OAuth 2.0 or OpenID Connect surface, and no\n  self-service\
  \ key issuance beyond the USOS form.\nschemes:\n- name: oauth1a\n  type: apiKey\n  in: query\n  parameter: oauth_token\n  api: university-of-warsaw:university-of-warsaw-apiref-api\n  description: >-\n    The USOS API uses OAuth 1.0a for authorized methods. A Consumer Key/Secret is obtained from the\n    USOS developers portal (https://usosapps.uw.edu.pl/developers/ — the page renders the real\n    registration form but answers HTTP 403 to non-browser clients), and an access token is obtained\n    via the flow documented at https://usosapps.uw.edu.pl/developers/api/authorization/ (200).\n    Anonymous methods such as services/apisrv/now and services/apiref/method_index need none of it.\n  sources:\n  - openapi/_original/university-of-warsaw-usos-api.yaml\n  - https://usosapps.uw.edu.pl/developers/api/authorization/\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  api: university-of-warsaw:sp4eu-api\n  description: >-\n    The Student Portal 4EU+ API declares\
  \ a single securityScheme, \"Authorization\" (apiKey, in\n    header). Its 401 body is the only public documentation of the flow: \"Please use /access/login\n    endpoint to receive bearer token. Api key should be provided as header: Authorization: Bearer\n    $BEARER_VALUE\". Read endpoints such as GET /api/v1/Tutorial answer without it; the Admin\n    subtree additionally role-gates and returns 403 \"Access Denied\".\n  sources:\n  - openapi/_original/university-of-warsaw-sp4eu-api.json\n  - https://api.sp4eu.uw.edu.pl/principal\n- name: bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  api: university-of-warsaw:jaskier-api\n  description: >-\n    Jaskier declares the same single \"Authorization\" apiKey header scheme. Every data endpoint\n    probed anonymously returned 401; only /v3/api-docs and /api/v1/system/build are open. No\n    public token-issuance path was found — the audience is the university's own applications.\n  sources:\n  - openapi/_original/university-of-warsaw-jaskier-api.json\n\
  - name: saml\n  type: federated\n  in: browser\n  parameter: SAMLResponse\n  api: university-of-warsaw:saml-idp\n  description: >-\n    End-user authentication for the portals is federated SAML 2.0 against the university's own\n    Shibboleth IdP, entityID https://login.uw.edu.pl/idp (metadata served at that URL, shibmd:Scope\n    login.uw.edu.pl), fronted by an Apereo CAS login at logowanie.uw.edu.pl and registered in\n    eduGAIN by PIONIER.Id. The Student Portal 4EU+ ships its own SP metadata at\n    https://api.sp4eu.uw.edu.pl/saml2/service-provider-metadata and exposes /principal/edugain.\n  sources:\n  - https://login.uw.edu.pl/idp\n  - https://api.sp4eu.uw.edu.pl/saml2/service-provider-metadata\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/authentication/university-of-warsaw-authentication.yml
summary_line: apiKey/oauth1a/bearer/saml · 4 schemes
tags:
- Education
- Higher Education
- University
- Poland
- Europe
- 4EU+ Alliance
- Academic Data
- Course Catalog
- Research Data
- Research Repository
- Identity Federation
- Library
- Open Data
---
