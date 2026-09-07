---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Authentication profile for the two ERS API surfaces. Derived from documentation rather than from a securitySchemes block, because ERS publishes no OpenAPI. The two surfaces do not share an auth model: the ARMS Data API is key-gated through the shared Federal api.data.gov gateway, and the geospatial ArcGIS services are anonymous.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Economic Research Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Economic Research Service declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Economic Research Service
provider_slug: economic-research-service
scheme_count: 0
schemes: []
slug: economic-research-service-authentication
source_filename: economic-research-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.ers.usda.gov/developer/data-apis/arms-data-api and\n  https://api.data.gov/docs/developer-manual/ (API Key Usage), plus a live unauthenticated\n  request to https://api.ers.usda.gov/data/arms/year on 2026-09-06 that returned HTTP 403\n  API_KEY_MISSING, and https://gisportal.ers.usda.gov/server/rest/info?f=json.\nprovider: Economic Research Service\nproviderId: economic-research-service\ndescription: >-\n  Authentication profile for the two ERS API surfaces. Derived from documentation rather than\n  from a securitySchemes block, because ERS publishes no OpenAPI. The two surfaces do not share\n  an auth model: the ARMS Data API is key-gated through the shared Federal api.data.gov\n  gateway, and the geospatial ArcGIS services are anonymous.\napis:\n  - api: USDA ERS Data APIs\n    aid: economic-research-service:ers-data-apis\n    baseURL: https://api.ers.usda.gov/data\n    auth_required: true\n    schemes:\n\
  \      - id: api_key_query\n        type: apiKey\n        in: query\n        name: api_key\n        primary: true\n        description: >-\n          The form ERS documents in every ARMS example, e.g.\n          GET https://api.ers.usda.gov/data/arms/year?api_key=YOUR_API_KEY. api.data.gov notes\n          the query parameter may be used for non-GET requests such as POST.\n        source: https://www.ers.usda.gov/developer/data-apis/arms-data-api\n      - id: api_key_header\n        type: apiKey\n        in: header\n        name: X-Api-Key\n        primary: false\n        description: >-\n          Platform-level alternative documented by api.data.gov for every API behind the\n          gateway. Not shown in ERS's own examples, but accepted by the gateway that fronts\n          api.ers.usda.gov.\n        source: https://api.data.gov/docs/developer-manual/\n      - id: http_basic_username\n        type: http\n        scheme: basic\n        primary: false\n        description: >-\n     \
  \     Platform-level alternative: the API key passed as the HTTP basic auth username with\n          an empty password. Documented by api.data.gov, not by ERS.\n        source: https://api.data.gov/docs/developer-manual/\n    credential:\n      issuer: api.data.gov\n      signup: https://api.data.gov/signup/\n      cost: free\n      approval: automatic, delivered by email\n      format: 40-character string\n      scope: >-\n        One key works across every agency API on api.data.gov, and the 1,000/hour limit is\n        shared across all of them - the key is not scoped to ERS.\n      rotation: not documented\n      revocation: >-\n        api.data.gov documents an API_KEY_DISABLED state administered by the platform; no\n        self-service rotation or revocation flow is published.\n    oauth2: false\n    oidc: false\n    mtls: false\n    unauthenticated_response:\n      status: 403\n      body: '{\"error\":{\"code\":\"API_KEY_MISSING\",\"message\":\"No api_key was supplied. Get one\
  \ at https://api.ers.usda.gov:443\"}}'\n      observed: '2026-09-06'\n      note: >-\n        Note that a missing credential returns 403, not 401, and carries no WWW-Authenticate\n        header - an agent cannot discover the auth scheme from the challenge.\n  - api: USDA ERS Geospatial APIs\n    aid: economic-research-service:ers-geospatial-apis\n    baseURL: https://gisportal.ers.usda.gov/server/rest/services\n    auth_required: false\n    schemes: []\n    description: >-\n      The published ArcGIS Server map, feature and image services answer anonymously over both\n      REST (?f=json) and SOAP (?wsdl). ArcGIS Server reports isTokenBasedSecurity true at\n      https://gisportal.ers.usda.gov/server/rest/info?f=json with a token endpoint at\n      https://gisportal.ers.usda.gov/portal/sharing/rest/generateToken, but that governs the\n      portal's own administrative and private content, not the public services ERS documents.\n    token_service: https://gisportal.ers.usda.gov/portal/sharing/rest/generateToken\n\
  consent_identity:\n  delegated_identity: false\n  end_user_consent: not applicable\n  note: >-\n    There is no user-scoped identity anywhere in this surface. The api.data.gov key identifies a\n    developer for rate-limiting and notification, not an end user, and no ERS API returns\n    user-owned data.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economic-research-service/refs/heads/main/authentication/economic-research-service-authentication.yml
summary_line: 0 schemes
tags:
- Agriculture
- Economics
- Federal-Government
- Research
- Open-Data
- Geospatial
- Statistics
---
