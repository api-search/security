---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Parse Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parse Biosciences declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Parse Biosciences
provider_slug: parse-biosciences
scheme_count: 0
schemes: []
slug: parse-biosciences-authentication
source_filename: parse-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://app.trailmaker.parsebiosciences.com/landing (the __NEXT_DATA__ amplifyConfig block\n  Parse Biosciences serves in its own application shell) plus the resulting Cognito OIDC\n  discovery document at\n  https://cognito-idp.eu-west-1.amazonaws.com/eu-west-1_eYTCV3Nl7/.well-known/openid-configuration\n  and a 401 observed on https://api.app.trailmaker.parsebiosciences.com/v2/experiments/examples\ndocs: null\n\nsummary: >-\n  Parse Biosciences publishes no developer API and therefore no developer authentication\n  documentation. It does operate one authenticated HTTP surface: the backend of Trailmaker,\n  its cloud single-cell data-analysis application. That backend is protected by AWS Cognito\n  (OIDC) and requires a bearer token; there is no public reference, no key-issuance flow, and\n  no published contract for it. Everything below was observed anonymously — no credentials\n  were used and no access control was defeated.\n\
  \npublic_developer_api: false\npublic_auth_documentation: false\n\nsurfaces:\n  - name: Trailmaker application backend\n    base_url: https://api.app.trailmaker.parsebiosciences.com\n    human_url: https://www.parsebiosciences.com/data-analysis/\n    status: live\n    audience: >-\n      First-party — this is the API the Trailmaker web client calls. It is not marketed,\n      documented, or offered to third-party developers.\n    evidence:\n      - url: https://api.app.trailmaker.parsebiosciences.com/v2/experiments/examples\n        http_status: 401\n        content_type: application/json; charset=utf-8\n        body: '{\"message\":\"The request does not contain an authentication token.\"}'\n      - url: https://api.app.trailmaker.parsebiosciences.com/v2/openapi.json\n        http_status: 404\n        body: '{\"message\":\"not found\"}'\n    observed_headers:\n      - x-powered-by: Express\n      - strict-transport-security: max-age=31536000; includeSubDomains\n      - access-control-allow-credentials:\
  \ 'true'\n      - access-control-expose-headers: X-Amzn-Trace-Id\n      - vary: Origin\n\nsecurity_schemes:\n  - id: cognito_oidc\n    type: openIdConnect\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    description: >-\n      Amazon Cognito user pool eu-west-1_eYTCV3Nl7 in eu-west-1, web client\n      665t39tl77h7q94f6ssvojmh77, authentication flow USER_SRP_AUTH. The application also\n      carries an unauthenticated Cognito identity pool\n      (eu-west-1:da43db0f-f5db-4276-a15b-614d606585e8) for pre-sign-in AWS calls.\n    openid_connect_url: >-\n      https://cognito-idp.eu-west-1.amazonaws.com/eu-west-1_eYTCV3Nl7/.well-known/openid-configuration\n    issuer: https://cognito-idp.eu-west-1.amazonaws.com/eu-west-1_eYTCV3Nl7\n    authorization_endpoint: >-\n      https://biomage-auth-production-242905224710.auth.eu-west-1.amazoncognito.com/oauth2/authorize\n    token_endpoint: >-\n      https://biomage-auth-production-242905224710.auth.eu-west-1.amazoncognito.com/oauth2/token\n\
  \    userinfo_endpoint: >-\n      https://biomage-auth-production-242905224710.auth.eu-west-1.amazoncognito.com/oauth2/userInfo\n    revocation_endpoint: >-\n      https://biomage-auth-production-242905224710.auth.eu-west-1.amazoncognito.com/oauth2/revoke\n    end_session_endpoint: >-\n      https://biomage-auth-production-242905224710.auth.eu-west-1.amazoncognito.com/logout\n    jwks_uri: >-\n      https://cognito-idp.eu-west-1.amazonaws.com/eu-west-1_eYTCV3Nl7/.well-known/jwks.json\n    response_types_supported: [code, token]\n    grant_types: [authorization_code]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n    scopes_supported:\n      - openid\n      - email\n      - phone\n      - profile\n    scopes_requested_by_trailmaker:\n      - aws.cognito.signin.user.admin\n      - email\n      - openid\n      - phone\n      - profile\n    redirect_sign_in: https://app.trailmaker.parsebiosciences.com/redirect\n\
  \    redirect_sign_out: https://app.trailmaker.parsebiosciences.com/landing/\n    saved_document: well-known/parse-biosciences-trailmaker-openid-configuration.json\n\napi_keys: none_published\noauth_client_registration: none_published\nmtls: false\n\nuser_facing_credentials:\n  - name: Trailmaker upload token\n    description: >-\n      Parse's Support Suite documents a command-line FASTQ upload path in which the user\n      downloads a \"parse-upload\" Python script from Trailmaker, generates a token in the\n      Trailmaker UI, and pastes the generated command into a console. The token is generated\n      per-session inside the signed-in application; neither the script nor a token format is\n      published at a public URL, and no token values are recorded here.\n    source: >-\n      https://support.parsebiosciences.com/hc/en-us/articles/27076682137236-Trailmaker-User-Guide\n    public: false\n\nnotes:\n  - >-\n    Trailmaker is a deployment of the open-source Cellenics/Biomage single-cell\
  \ platform\n    (github.com/hms-dbmi-cellenics). The evidence is in Parse's own served config: the Cognito\n    hosted-UI domain is literally biomage-auth-production-242905224710, analytics point at\n    biomage.matomo.cloud, and the Trailmaker course site is biomage-s-site.thinkific.com. The\n    upstream project publishes an OpenAPI for this API — but that spec belongs to Cellenics\n    (info.title \"API\", contact.name \"Cellenics\", MIT, servers \"/v2\", hosted in the HMS DBMI\n    org), not to Parse Biosciences, so it is deliberately NOT harvested into this repo. See\n    the ownership note in conventions/parse-biosciences-conventions.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parse-biosciences/refs/heads/main/authentication/parse-biosciences-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Genomics
- Single-Cell Sequencing
- Bioinformatics
- Scientific Software
- Data Analysis
- Laboratory
- Research
---
