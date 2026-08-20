---
api_key_in: []
api_specs:
- filename: google-analytics-accounts-api-openapi.yml
  format: yaml
  label: Google Analytics accounts API
  slug: google-analytics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accounts-api-openapi.yml
- filename: google-analytics-accountsummaries-api-openapi.yml
  format: yaml
  label: Google Analytics accountSummaries API
  slug: google-analytics-accountsummaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-accountsummaries-api-openapi.yml
- filename: google-analytics-data-api-openapi.yml
  format: yaml
  label: Google Analytics data API
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-data-api-openapi.yml
- filename: google-analytics-events-api-openapi.yml
  format: yaml
  label: Google Analytics Events API
  slug: google-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-events-api-openapi.yml
- filename: google-analytics-management-api-openapi.yml
  format: yaml
  label: Google Analytics management API
  slug: google-analytics-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-management-api-openapi.yml
- filename: google-analytics-metadata-api-openapi.yml
  format: yaml
  label: Google Analytics metadata API
  slug: google-analytics-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-metadata-api-openapi.yml
- filename: google-analytics-properties-api-openapi.yml
  format: yaml
  label: Google Analytics properties API
  slug: google-analytics-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-properties-api-openapi.yml
- filename: google-analytics-provisioning-api-openapi.yml
  format: yaml
  label: Google Analytics provisioning API
  slug: google-analytics-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-provisioning-api-openapi.yml
- filename: google-analytics-reports-api-openapi.yml
  format: yaml
  label: Google Analytics reports API
  slug: google-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-reports-api-openapi.yml
- filename: google-analytics-user-deletion-api-openapi.yml
  format: yaml
  label: Google Analytics User Deletion API
  slug: google-analytics-user-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-user-deletion-api-openapi.yml
- filename: google-analytics-useractivity-api-openapi.yml
  format: yaml
  label: Google Analytics userActivity API
  slug: google-analytics-useractivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-useractivity-api-openapi.yml
- filename: google-analytics-userdeletion-api-openapi.yml
  format: yaml
  label: Google Analytics userDeletion API
  slug: google-analytics-userdeletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-userdeletion-api-openapi.yml
- filename: google-analytics-validation-api-openapi.yml
  format: yaml
  label: Google Analytics Validation API
  slug: google-analytics-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-validation-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Google Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- jwt-bearer (service account)
- device_code
overview: Google Analytics secures its APIs with oauth2 and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, jwt-bearer (service account), and device_code flow(s).
provider_name: Google Analytics
provider_slug: google-analytics
scheme_count: 5
schemes:
- applies_to:
  - Google Analytics Data API
  - Google Analytics Admin API
  authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth
  flow: authorizationCode
  header: 'Authorization: Bearer <access_token>'
  name: OAuth 2.0 user credentials (authorization code)
  note: The legacy endpoint https://accounts.google.com/o/oauth2/auth still appears in the OpenAPI securitySchemes; the current discovery document publishes https://accounts.google.com/o/oauth2/v2/auth.
  refresh: true
  revocation_endpoint: https://oauth2.googleapis.com/revoke
  token_endpoint: https://oauth2.googleapis.com/token
  type: oauth2
- applies_to:
  - Google Analytics Data API
  - Google Analytics Admin API
  authorization_endpoint: https://accounts.google.com/o/oauth2/auth
  deprecated: true
  flow: implicit
  name: OAuth 2.0 implicit
  note: Declared in the OpenAPI securitySchemes but discouraged by Google; the implicit grant is not recommended for new integrations.
  type: oauth2
- applies_to:
  - Google Analytics Data API
  - Google Analytics Admin API
  flow: urn:ietf:params:oauth:grant-type:jwt-bearer
  name: Service account / Application Default Credentials
  note: This is the production pattern for server-to-server access and the only path Google's own MCP server supports.
  setup: gcloud auth application-default login --scopes https://www.googleapis.com/auth/analytics.readonly,https://www.googleapis.com/auth/cloud-platform — or a service-account key file referenced by GOOGLE_APPLICATION_CREDENTIALS. The service account's email must then be granted a role on the Google Analytics property in the Analytics UI; enabling the API is not enough.
  type: oauth2
- api_managed: 'Also creatable through the Admin API: properties.dataStreams.measurementProtocolSecrets.create'
  applies_to:
  - Measurement Protocol (GA4)
  companion_parameters:
  - measurement_id (web streams)
  - firebase_app_id (app streams)
  in: query
  minted_at: Google Analytics UI > Admin > Data collection and modification > Data streams > select stream > Measurement Protocol API secrets > Create
  name: Measurement Protocol api_secret
  parameter: api_secret
  risk: A bearer secret in a query string. Google's docs warn explicitly that exposing it lets anyone inject arbitrary or spam events into the property and corrupt its reporting. It grants write-only ingestion — it cannot read data.
  rotation: Multiple secrets can exist per stream, so rotation is create-new-then-delete-old. No expiry, no automatic rotation.
  type: apiKey
- applies_to:
  - Google Analytics Data API
  - Google Analytics Admin API
  in: query
  name: Google Cloud API key
  note: Identifies the calling Google Cloud project for quota and billing. It is NOT an authorization mechanism — an API key alone cannot access any property's data.
  parameter: key
  type: apiKey
slug: google-analytics-authentication
source_filename: google-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.google.com/analytics/devguides/reporting/data/v1/quickstart-client-libraries,\n  https://developers.google.com/analytics/devguides/collection/protocol/ga4/sending-events\n  and https://developers.google.com/analytics/devguides/config/userdeletion/v3/authorization\n  (fetched 2026-08-13), plus the live metadata at\n  https://accounts.google.com/.well-known/openid-configuration and\n  .../oauth-authorization-server (both HTTP 200, saved under well-known/), and the\n  securitySchemes declared in openapi/_original/*.yaml\nprovider: Google Analytics\nproviderId: google-analytics\nsupersedes: >-\n  The 2026-07-11 derived version, which reported only the two OpenAPI oauth2 schemes\n  (implicit + authorizationCode) and missed both the Measurement Protocol shared\n  secret and the service-account/ADC path that is the actual production pattern.\nsummary:\n  types:\n    - oauth2\n    - apiKey\n  oauth2_flows:\n\
  \    - authorizationCode\n    - implicit\n    - jwt-bearer (service account)\n    - device_code\n  transport: HTTPS only (TLS 1.3 observed on all API hosts)\nschemes:\n  - name: OAuth 2.0 user credentials (authorization code)\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint: https://accounts.google.com/o/oauth2/v2/auth\n    token_endpoint: https://oauth2.googleapis.com/token\n    revocation_endpoint: https://oauth2.googleapis.com/revoke\n    header: 'Authorization: Bearer <access_token>'\n    refresh: true\n    applies_to:\n      - Google Analytics Data API\n      - Google Analytics Admin API\n    note: >-\n      The legacy endpoint https://accounts.google.com/o/oauth2/auth still appears in\n      the OpenAPI securitySchemes; the current discovery document publishes\n      https://accounts.google.com/o/oauth2/v2/auth.\n  - name: OAuth 2.0 implicit\n    type: oauth2\n    flow: implicit\n    authorization_endpoint: https://accounts.google.com/o/oauth2/auth\n   \
  \ applies_to:\n      - Google Analytics Data API\n      - Google Analytics Admin API\n    deprecated: true\n    note: >-\n      Declared in the OpenAPI securitySchemes but discouraged by Google; the implicit\n      grant is not recommended for new integrations.\n  - name: Service account / Application Default Credentials\n    type: oauth2\n    flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    applies_to:\n      - Google Analytics Data API\n      - Google Analytics Admin API\n    setup: >-\n      gcloud auth application-default login --scopes\n      https://www.googleapis.com/auth/analytics.readonly,https://www.googleapis.com/auth/cloud-platform\n      — or a service-account key file referenced by GOOGLE_APPLICATION_CREDENTIALS.\n      The service account's email must then be granted a role on the Google\n      Analytics property in the Analytics UI; enabling the API is not enough.\n    note: >-\n      This is the production pattern for server-to-server access and the only path\n\
  \      Google's own MCP server supports.\n  - name: Measurement Protocol api_secret\n    type: apiKey\n    in: query\n    parameter: api_secret\n    companion_parameters:\n      - measurement_id (web streams)\n      - firebase_app_id (app streams)\n    applies_to:\n      - Measurement Protocol (GA4)\n    minted_at: >-\n      Google Analytics UI > Admin > Data collection and modification > Data streams >\n      select stream > Measurement Protocol API secrets > Create\n    api_managed: >-\n      Also creatable through the Admin API:\n      properties.dataStreams.measurementProtocolSecrets.create\n    rotation: >-\n      Multiple secrets can exist per stream, so rotation is create-new-then-delete-old.\n      No expiry, no automatic rotation.\n    risk: >-\n      A bearer secret in a query string. Google's docs warn explicitly that exposing\n      it lets anyone inject arbitrary or spam events into the property and corrupt\n      its reporting. It grants write-only ingestion — it cannot read\
  \ data.\n  - name: Google Cloud API key\n    type: apiKey\n    in: query\n    parameter: key\n    applies_to:\n      - Google Analytics Data API\n      - Google Analytics Admin API\n    note: >-\n      Identifies the calling Google Cloud project for quota and billing. It is NOT an\n      authorization mechanism — an API key alone cannot access any property's data.\nauthorization_model:\n  description: >-\n    Two independent gates, and both must pass. (1) The Google Cloud project must have\n    the Google Analytics Admin API and/or Data API enabled. (2) The calling identity\n    — user or service account — must hold a Google Analytics role on the target\n    property, granted in the Analytics UI or through Admin API access bindings. OAuth\n    scope is a third, coarse filter on top of both.\n  common_failure: >-\n    HTTP 403 PERMISSION_DENIED with the API enabled and the token valid almost always\n    means step (2) was skipped — the service account was never added to the property.\n\
  mtls:\n  supported: false\nscopes: scopes/google-analytics-scopes.yml\nwell_known:\n  openid_configuration: well-known/google-analytics-openid-configuration.json\n  oauth_authorization_server: well-known/google-analytics-oauth-authorization-server.json\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/authentication/google-analytics-authentication.yml
summary_line: oauth2/apiKey · 5 schemes
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine-Learning
- Attribution
---
