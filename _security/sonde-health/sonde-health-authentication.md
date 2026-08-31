---
api_key_in:
- header
api_specs:
- filename: sonde-health-screening-api-openapi.yaml
  format: yaml
  label: Sonde Screening API
  slug: sonde-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/openapi/sonde-health-screening-api-openapi.yaml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Sonde Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonde Health secures its APIs with oauth2 and apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sonde Health
provider_slug: sonde-health
scheme_count: 1
schemes:
- authorizer:
    declared_in: openapi/sonde-health-screening-api-openapi.yaml
    type: cognito_user_pools
  bearer_header: 'Authorization: <access_token>'
  client_authentication: 'HTTP Basic — Authorization: Basic base64(client-id:client-secret). The docs show `echo -n "<client-id>:<client-secret>" | openssl base64 -A`.'
  expires_in_seconds: 3600
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2
  request_content_type: application/x-www-form-urlencoded
  scopes_ref: scopes/sonde-health-scopes.yml
  sources:
  - https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706702379/Mental+Fitness+Voice+Features+API
  - openapi/sonde-health-screening-api-openapi.yaml
  token_type: Bearer
  token_url: https://api.sondeservices.com/platform/v1/oauth2/token
  token_url_screening_api: https://api.sondeservices.com/platform/api/v1/oauth2/token
  type: oauth2
slug: sonde-health-authentication
source_filename: sonde-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\ndocs:\n- https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706931713/Authentication+Scopes\n- https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706702379/Mental+Fitness+Voice+Features+API\n- https://sondehealth.atlassian.net/wiki/spaces/SPPA/pages/1614250108/REST+API+Reference\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  primary: oauth2-client-credentials\n  api_key_in:\n  - header\n  note: >-\n    The published OpenAPI declares the scheme as `type: apiKey` in the Authorization\n    header, but the underlying mechanism the docs describe is OAuth 2.0\n    client_credentials fronted by an Amazon Cognito user pool\n    (x-amazon-apigateway-authtype: cognito_user_pools). Both facts are recorded here\n    rather than picking one.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.sondeservices.com/platform/v1/oauth2/token\n\
  \  token_url_screening_api: https://api.sondeservices.com/platform/api/v1/oauth2/token\n  client_authentication: >-\n    HTTP Basic — Authorization: Basic base64(client-id:client-secret). The docs show\n    `echo -n \"<client-id>:<client-secret>\" | openssl base64 -A`.\n  request_content_type: application/x-www-form-urlencoded\n  grant_type: client_credentials\n  token_type: Bearer\n  expires_in_seconds: 3600\n  bearer_header: 'Authorization: <access_token>'\n  scopes_ref: scopes/sonde-health-scopes.yml\n  authorizer:\n    type: cognito_user_pools\n    declared_in: openapi/sonde-health-screening-api-openapi.yaml\n  sources:\n  - https://sondehealth.atlassian.net/wiki/spaces/SA/pages/2706702379/Mental+Fitness+Voice+Features+API\n  - openapi/sonde-health-screening-api-openapi.yaml\ncredential_issuance:\n  self_service: false\n  process: >-\n    Credentials (client-id / client-secret) are issued by Sonde during partner\n    registration/onboarding; scopes are allocated per contract. There\
  \ is no public\n    self-service key issuance.\n  contact: support@sondehealth.com\n  registration_docs: https://sondehealth.atlassian.net/wiki/spaces/BAC/pages/2987622403/Sonde+Health+API+Platform+Portal+-+Registration+flow\n  registration_docs_gated: true\n  registration_docs_probe:\n    fetched: '2026-08-28'\n    http_status: 200\n    detail: >-\n      Sonde's public support page links this \"API Platform Portal - Registration flow\"\n      page, but the BAC Confluence space is restricted: the URL returns 200 carrying an\n      Atlassian login prompt rather than the registration instructions, and the\n      Confluence content API returns an empty body for the page id. The two\n      documentation spaces that ARE public are SA (Sonde Health Platform Documentation)\n      and SPPA (Sonde Product Partner API).\n  partner_portal: https://us.sondeservices.com/\nsdk_authentication:\n  note: >-\n    The Android/iOS Passive and Edge SDKs initialise with clientId, clientSecret and\n    an optional\
  \ clientCode rather than a bearer token.\n  source: https://sondehealth.atlassian.net/wiki/spaces/SA/pages/3303899168/Android+SDK+Initialization\nguidance:\n  - Keep client-credentials server-side; the docs explicitly warn against shipping them\n    in client-side code or public repositories.\n  - Mint a narrowly scoped token per device task (e.g. only sonde-platform/storage.write\n    for an upload) rather than sharing a full-privilege token with a handset.\n  - Tokens expire after 3600 seconds and must be re-fetched by the partner backend.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonde-health/refs/heads/main/authentication/sonde-health-authentication.yml
summary_line: oauth2/apiKey · 1 scheme
tags:
- Company
- Health
- Healthcare
- Digital Health
- Vocal Biomarkers
- Voice
- Audio
- Machine-Learning
- Artificial Intelligence
- Mental Health
- Respiratory
- Remote Patient Monitoring
- Wellness
- HIPAA
---
