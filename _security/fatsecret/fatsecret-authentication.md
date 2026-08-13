---
api_key_in: []
api_specs:
- filename: fatsecret-exercise-diary-api-openapi.yml
  format: yaml
  label: fatsecret Exercise Diary API
  slug: fatsecret-exercise-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-exercise-diary-api-openapi.yml
- filename: fatsecret-food-diary-api-openapi.yml
  format: yaml
  label: fatsecret Food Diary API
  slug: fatsecret-food-diary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-food-diary-api-openapi.yml
- filename: fatsecret-foods-api-openapi.yml
  format: yaml
  label: fatsecret Foods API
  slug: fatsecret-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-foods-api-openapi.yml
- filename: fatsecret-image-recognition-api-openapi.yml
  format: yaml
  label: fatsecret Image Recognition API
  slug: fatsecret-image-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-image-recognition-api-openapi.yml
- filename: fatsecret-natural-language-processing-api-openapi.yml
  format: yaml
  label: fatsecret Natural Language Processing API
  slug: fatsecret-natural-language-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-natural-language-processing-api-openapi.yml
- filename: fatsecret-profile-foods-api-openapi.yml
  format: yaml
  label: fatsecret Profile Foods API
  slug: fatsecret-profile-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-foods-api-openapi.yml
- filename: fatsecret-profile-meals-api-openapi.yml
  format: yaml
  label: fatsecret Profile Meals API
  slug: fatsecret-profile-meals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-profile-meals-api-openapi.yml
- filename: fatsecret-recipes-api-openapi.yml
  format: yaml
  label: fatsecret Recipes API
  slug: fatsecret-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-recipes-api-openapi.yml
- filename: fatsecret-reference-api-openapi.yml
  format: yaml
  label: fatsecret Reference API
  slug: fatsecret-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-reference-api-openapi.yml
- filename: fatsecret-weight-tracking-api-openapi.yml
  format: yaml
  label: fatsecret Weight Tracking API
  slug: fatsecret-weight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/openapi/fatsecret-weight-tracking-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fatsecret Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: fatsecret secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: fatsecret
provider_slug: fatsecret
scheme_count: 2
schemes:
- credential: Consumer Key (client_id) + Consumer Secret (client_secret) issued at registration
  flows:
  - flow: clientCredentials
    scope_list:
    - basic
    - premier
    - barcode
    - localization
    - nlp
    - image-recognition
    - feedback
    scopes: 7
    tokenUrl: https://oauth.fatsecret.com/connect/token
  name: oauth2
  provider_guidance: '"fatsecret requires that OAuth 2.0 tokens be requested through a proxy server" — the secret must not ship in a mobile or browser client.'
  request_header: 'Authorization: Bearer <access_token>'
  sources:
  - openapi/_original/fatsecret-platform-openapi.yml
  - https://platform.fatsecret.com/docs/guides/authentication/oauth2
  token_lifetime: 24 hours (default)
  type: oauth2
- description: OAuth 1.0a request signing; 3-legged for member-scoped data
  name: oauth1
  note: The profile is carried by the access token, not by a user_id parameter. OAuth 1.0a signing errors are reported as fatsecret error codes 2-9, not as HTTP 401.
  scheme: oauth
  scopes: 0
  signature_methods_documented: true
  sources:
  - openapi/_original/fatsecret-platform-openapi.yml
  - https://platform.fatsecret.com/docs/guides/authentication/oauth1/three-legged
  type: http
slug: fatsecret-authentication
source_filename: fatsecret-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://platform.fatsecret.com/docs/guides/authentication\ndocs:\n  index: https://platform.fatsecret.com/docs/guides/authentication\n  oauth2: https://platform.fatsecret.com/docs/guides/authentication/oauth2\n  oauth1: https://platform.fatsecret.com/docs/guides/authentication/oauth1\n  oauth1_three_legged: https://platform.fatsecret.com/docs/guides/authentication/oauth1/three-legged\nnote: >-\n  Upgraded from derived to searched on 2026-08-12 with the provider's auth guides and a live probe of\n  the authorization server's OIDC discovery document.\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  two_plane: >-\n    Two authentication planes that are not interchangeable. Catalog data (foods, recipes, reference)\n    uses OAuth 2.0 client_credentials — an APPLICATION identity. Member data (food diary, exercise\n    diary, weight, favorites, saved meals) uses 3-legged OAuth 1.0a — a\
  \ MEMBER identity. An agent\n    holding only a client-credentials token cannot read or write any profile surface.\nauthorization_server:\n  issuer: https://oauth.fatsecret.com\n  openid_configuration: https://oauth.fatsecret.com/.well-known/openid-configuration\n  probed: '2026-08-12'\n  http_status: 200\n  endpoints:\n    authorization: https://oauth.fatsecret.com/connect/authorize\n    token: https://oauth.fatsecret.com/connect/token\n    userinfo: https://oauth.fatsecret.com/connect/userinfo\n    introspection: https://oauth.fatsecret.com/connect/introspect\n    revocation: https://oauth.fatsecret.com/connect/revocation\n    device_authorization: https://oauth.fatsecret.com/connect/deviceauthorization\n    end_session: https://oauth.fatsecret.com/connect/endsession\n    jwks: https://oauth.fatsecret.com/.well-known/openid-configuration/jwks\n  id_token_signing_alg: [RS256]\n  code_challenge_methods: [plain, S256]\n  subject_types: [public]\nschemes:\n  - name: oauth2\n    type: oauth2\n\
  \    flows:\n      - flow: clientCredentials\n        tokenUrl: https://oauth.fatsecret.com/connect/token\n        scopes: 7\n        scope_list: [basic, premier, barcode, localization, nlp, image-recognition, feedback]\n    credential: Consumer Key (client_id) + Consumer Secret (client_secret) issued at registration\n    request_header: 'Authorization: Bearer <access_token>'\n    token_lifetime: 24 hours (default)\n    provider_guidance: >-\n      \"fatsecret requires that OAuth 2.0 tokens be requested through a proxy server\" — the secret must\n      not ship in a mobile or browser client.\n    sources:\n      - openapi/_original/fatsecret-platform-openapi.yml\n      - https://platform.fatsecret.com/docs/guides/authentication/oauth2\n  - name: oauth1\n    type: http\n    scheme: oauth\n    description: OAuth 1.0a request signing; 3-legged for member-scoped data\n    signature_methods_documented: true\n    scopes: 0\n    sources:\n      - openapi/_original/fatsecret-platform-openapi.yml\n\
  \      - https://platform.fatsecret.com/docs/guides/authentication/oauth1/three-legged\n    note: >-\n      The profile is carried by the access token, not by a user_id parameter. OAuth 1.0a signing\n      errors are reported as fatsecret error codes 2-9, not as HTTP 401.\nip_restriction:\n  supported: true\n  evidence: error code 21, \"Invalid IP address detected\"\nsee_also:\n  scopes: scopes/fatsecret-scopes.yml\n  errors: errors/fatsecret-error-codes.yml\n  conventions: conventions/fatsecret-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/authentication/fatsecret-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Artificial Intelligence
- Barcode Scanning
- Calories
- Diets
- Image Recognition
- Natural Language Processing
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
---
