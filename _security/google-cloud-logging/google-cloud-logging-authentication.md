---
anonymous_access: false
api_key_in: []
api_specs:
- filename: google-cloud-logging-bucket-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Bucket API
  slug: google-cloud-logging-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-bucket-api-openapi.yml
- filename: google-cloud-logging-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Buckets API
  slug: google-cloud-logging-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-buckets-api-openapi.yml
- filename: google-cloud-logging-entries-copy-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:copy API
  slug: google-cloud-logging-entries-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-copy-api-openapi.yml
- filename: google-cloud-logging-entries-list-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:list API
  slug: google-cloud-logging-entries-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-list-api-openapi.yml
- filename: google-cloud-logging-entries-tail-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:tail API
  slug: google-cloud-logging-entries-tail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-tail-api-openapi.yml
- filename: google-cloud-logging-entries-write-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:write API
  slug: google-cloud-logging-entries-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-write-api-openapi.yml
- filename: google-cloud-logging-exclusions-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Exclusions API
  slug: google-cloud-logging-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-exclusions-api-openapi.yml
- filename: google-cloud-logging-google-cloud-logging-api-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Google Cloud Logging API
  slug: google-cloud-logging-google-cloud-logging-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-google-cloud-logging-api-api-openapi.yml
- filename: google-cloud-logging-sinks-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Sinks API
  slug: google-cloud-logging-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-sinks-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Google Cloud Logging Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- service-account-jwt
- workload-identity-federation
overview: Google Cloud Logging secures its APIs with oauth2, openIdConnect, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, service-account-jwt, and workload-identity-federation flow(s).
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-cloud-logging-openapi.yml
  - discovery/google-cloud-logging-discovery-v2.json
  type: oauth2
- issuer: https://accounts.google.com
  jwks_uri: https://www.googleapis.com/oauth2/v3/certs
  name: GoogleOIDC
  openIdConnectUrl: https://accounts.google.com/.well-known/openid-configuration
  sources:
  - well-known/google-cloud-logging-openid-configuration.json
  type: openIdConnect
- endpoint: https://logging.mtls.googleapis.com/
  name: MutualTLS
  sources:
  - discovery/google-cloud-logging-discovery-v2.json
  type: mutualTLS
slug: google-cloud-logging-authentication
source_filename: google-cloud-logging-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: openapi/google-cloud-logging-openapi.yml\ndocs: https://docs.cloud.google.com/logging/docs/access-control\nadditional_docs:\n  - https://cloud.google.com/docs/authentication\n  - https://accounts.google.com/.well-known/openid-configuration\n  - https://accounts.google.com/.well-known/oauth-authorization-server\nnote: >-\n  Upgraded from the 2026-07-11 derived pass. The spec-derived baseline named only the\n  authorizationCode flow and four scopes; the Discovery document and Google's own auth docs\n  add the cloud-platform.read-only scope, the mTLS endpoint, and the service-account /\n  workload-identity-federation credential paths an actual integration uses. Both OAuth\n  discovery documents were fetched live on 2026-09-12 (HTTP 200) and saved under well-known/.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode, service-account-jwt, workload-identity-federation]\n  api_key_in: []\n \
  \ api_keys_supported: false\n  bearer_token: Authorization -> Bearer <OAuth 2.0 access token>\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        scopes: 5\n    sources: [openapi/google-cloud-logging-openapi.yml, discovery/google-cloud-logging-discovery-v2.json]\n  - name: GoogleOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://accounts.google.com/.well-known/openid-configuration\n    issuer: https://accounts.google.com\n    jwks_uri: https://www.googleapis.com/oauth2/v3/certs\n    sources: [well-known/google-cloud-logging-openid-configuration.json]\n  - name: MutualTLS\n    type: mutualTLS\n    endpoint: https://logging.mtls.googleapis.com/\n    sources: [discovery/google-cloud-logging-discovery-v2.json]\ncredential_types:\n  - type: user-oauth\n    note: Interactive authorizationCode flow, used by gcloud\
  \ auth login and by MCP clients.\n  - type: service-account\n    note: >-\n      Signed JWT exchanged for an access token — the normal server-to-server path. Preferred\n      form is Application Default Credentials rather than a downloaded key file.\n  - type: workload-identity-federation\n    note: Recommended over service-account key files for workloads outside Google Cloud.\n  - type: api-key\n    supported: false\n    note: >-\n      API keys do not authorize Cloud Logging calls. The MCP setup page mentions API keys as a\n      connection field, but authorization on the Logging surface is OAuth + IAM.\nauthorization:\n  model: Google Cloud IAM layered over the OAuth scope\n  note: >-\n    The scope decides what class of call the token may make; the IAM role on the resource\n    decides whether this principal may make it. Both must pass — a cloud-platform token with\n    no Logging role still gets 403 PERMISSION_DENIED.\n  roles:\n    - roles/logging.viewer\n    - roles/logging.privateLogViewer\n\
  \    - roles/logging.logWriter\n    - roles/logging.configWriter\n    - roles/logging.admin\n    - roles/mcp.toolUser\n  docs: https://docs.cloud.google.com/logging/docs/access-control\nscopes_detail: scopes/google-cloud-logging-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/authentication/google-cloud-logging-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 3 schemes
tags:
- Cloud
- Logging
- Monitoring
- Observability
- Telemetry
- Log Management
- SRE
- DevOps
- OpenTelemetry
- Google Cloud
---
