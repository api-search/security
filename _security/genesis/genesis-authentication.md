---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: genesis-catalogue-api-openapi.yml
  format: yaml
  label: GENESIS Catalogue API
  slug: genesis-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-catalogue-api-openapi.yml
- filename: genesis-data-api-openapi.yml
  format: yaml
  label: GENESIS Data API
  slug: genesis-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-data-api-openapi.yml
- filename: genesis-find-api-openapi.yml
  format: yaml
  label: GENESIS Find API
  slug: genesis-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-find-api-openapi.yml
- filename: genesis-helloworld-api-openapi.yml
  format: yaml
  label: GENESIS Helloworld API
  slug: genesis-helloworld-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-helloworld-api-openapi.yml
- filename: genesis-metadata-api-openapi.yml
  format: yaml
  label: GENESIS Metadata API
  slug: genesis-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-metadata-api-openapi.yml
- filename: genesis-profile-api-openapi.yml
  format: yaml
  label: GENESIS Profile API
  slug: genesis-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesis/openapi/genesis-profile-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GENESIS Authentication
name_suffix: Authentication
oauth_flows: []
overview: GENESIS secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GENESIS
provider_slug: genesis
scheme_count: 2
schemes:
- description: 'User Guide "Web Services" v5.1 s2.1.3: "With the exception of the whoami service, authentication is required for every request. This can be done via the combined entry of user name/email and password or via the personal token." Account data travel as HTTP header fields (form-urlencoded body also accepted). Only POST is served: "The SOAP/XML interface as well as GET methods of the RESTful/JSON interface have been switched off" (15.07.2025).'
  how_to_obtain: Free registration on GENESIS-Online (https://genesis.destatis.de/datenbank/online#modal=register).
  in: header
  name: username / password
  parameter: username, password
  sources:
  - openapi/_original/genesis-openapi.json
  - https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf
  type: apiKey
- description: 's2.1.3: "A personal API token is displayed in the ''Webservice (API)'' modal after logging in to the web interface. The token can be used in requests instead of the user name/email. It is no longer necessary to enter a password when using the token." 32 characters. Regenerating it invalidates the old one immediately. profile/removeresult, profile/password and job=true requests still require user name and password.'
  how_to_obtain: Log in to GENESIS-Online and open the "Webservice interface (API)" modal.
  in: header
  name: personal API token
  parameter: username
  sources:
  - https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf
  type: apiKey
slug: genesis-authentication
source_filename: genesis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf\ndocs: https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  registration_required: true\n  note: >-\n    TWO DIFFERENT ACCESS MODELS, and the destatis.de open-data page describes only the first. The\n    GENESIS-Online web interface (https://genesis.destatis.de/datenbank/online) \"can be used free of\n    charge and without registering\" under Data Licence Germany - Attribution - Version 2.0\n    (https://www.destatis.de/EN/Service/OpenData/api-webservice.html). The GENESIS web service\n    (RESTful/JSON API, https://genesis.destatis.de/genesisWS/rest/2020/...) does NOT accept anonymous\n    calls: \"Free registration in GENESIS-Online is required to use the web service. Each request\n    requires username and password\" (Webservice interface (API)\
  \ modal, served in\n    https://genesis.destatis.de/datenbank/online/environment.json). Registration is free. The contract\n    (openapi/_original/genesis-openapi.json) declares no securitySchemes; credentials are modelled as\n    `username` / `password` header parameters on every operation.\nschemes:\n- name: username / password\n  type: apiKey\n  in: header\n  parameter: username, password\n  sources:\n  - openapi/_original/genesis-openapi.json\n  - https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf\n  description: >-\n    User Guide \"Web Services\" v5.1 s2.1.3: \"With the exception of the whoami service, authentication\n    is required for every request. This can be done via the combined entry of user name/email and\n    password or via the personal token.\" Account data travel as HTTP header fields (form-urlencoded\n    body also accepted). Only POST is served: \"The SOAP/XML interface as well as GET methods of the\n    RESTful/JSON interface have\
  \ been switched off\" (15.07.2025).\n  how_to_obtain: Free registration on GENESIS-Online (https://genesis.destatis.de/datenbank/online#modal=register).\n- name: personal API token\n  type: apiKey\n  in: header\n  parameter: username\n  sources:\n  - https://genesis.destatis.de/datenbank/online/docs/GENESIS-Webservices_Introduction.pdf\n  description: >-\n    s2.1.3: \"A personal API token is displayed in the 'Webservice (API)' modal after logging in to the\n    web interface. The token can be used in requests instead of the user name/email. It is no longer\n    necessary to enter a password when using the token.\" 32 characters. Regenerating it invalidates the\n    old one immediately. profile/removeresult, profile/password and job=true requests still require\n    user name and password.\n  how_to_obtain: Log in to GENESIS-Online and open the \"Webservice interface (API)\" modal.\nevidence:\n- request: GET https://genesis.destatis.de/genesisWS/rest/2020/helloworld/logincheck (no credentials)\n\
  \  observed: '2026-11-11'\n  http_status: 405\n  detail: GET is switched off, as the documentation says.\n- request: POST https://genesis.destatis.de/genesisWS/rest/2020/catalogue/tables (no credentials; selection=12411*, language=en)\n  observed: '2026-11-11'\n  http_status: 401\n  detail: '{\"Code\":15,\"Content\":\"You are not allowed to call this service or the header of your request does\n    not contain all the necessary information so that your access data cannot be recognised.\",\"Type\":\"ERROR\"}'\n- request: POST https://genesis.destatis.de/genesisWS/rest/2020/helloworld/logincheck (no credentials)\n  observed: '2026-11-11'\n  http_status: 200\n  detail: '{\"Status\":\"You have been logged in and out successfully! ...\",\"Username\":\"GAST\"} -- an uncredentialed\n    logincheck is answered as the built-in guest user (the contract''s header defaults are GAST/GAST), but\n    the guest is refused by the data services (Code 15 above). No credentials were tried.'\nanonymous_routes_observed:\n\
  - POST /rest/2020/helloworld/logincheck (answers as guest \"GAST\"; tests nothing about data access)\n- POST /rest/2020/helloworld/whoami (documented as the one method needing no authentication; not called)\n"
source_yaml_url: https://artifacts.apis.io/genesis/authentication/genesis-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Open Data
- Public APIs
---
