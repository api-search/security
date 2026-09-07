---
anonymous_access: false
api_key_in: []
api_specs:
- filename: confluent-the-data-streaming-platform-cloud-apis-openapi.yml
  format: yaml
  label: Confluent Cloud REST API
  slug: cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
- filename: confluent-the-data-streaming-platform-api-keys-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform API Keys API
  slug: confluent-the-data-streaming-platform-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml
- filename: confluent-the-data-streaming-platform-clusters-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Clusters API
  slug: confluent-the-data-streaming-platform-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml
- filename: confluent-the-data-streaming-platform-environments-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Environments API
  slug: confluent-the-data-streaming-platform-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml
- filename: confluent-the-data-streaming-platform-organizations-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Organizations API
  slug: confluent-the-data-streaming-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml
- filename: confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
  format: yaml
  label: Confluent | the Data Streaming Platform Service Accounts API
  slug: confluent-the-data-streaming-platform-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Confluent The Data Streaming Platform Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Confluent | the Data Streaming Platform secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Confluent | the Data Streaming Platform
provider_slug: confluent-the-data-streaming-platform
scheme_count: 3
schemes:
- description: Cloud API Key (key) and Secret (password)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
  - openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
  type: http
- bearerFormat: JWT
  description: Confluent STS or external OAuth access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml
  - openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml
  type: http
- description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth 2.0.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token
  name: confluent-sts-access-token
  sources:
  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml
  type: oauth2
slug: confluent-the-data-streaming-platform-authentication
source_filename: confluent-the-data-streaming-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml, openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml,\n  openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml, openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml,\n  openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml, openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Cloud API Key (key) and Secret (password)\n  sources:\n  - openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml\n\
  \  - openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Confluent STS or external OAuth access token\n  sources:\n  - openapi/confluent-the-data-streaming-platform-api-keys-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-clusters-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-environments-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-organizations-api-openapi.yml\n  - openapi/confluent-the-data-streaming-platform-service-accounts-api-openapi.yml\n- name: confluent-sts-access-token\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.confluent.cloud/sts/v1/oauth2/token\n    scopes: 0\n  description: Authenticate with Confluent API using this credentials (JSON Web Tokens) following OAuth\n    2.0.\n  sources:\n\
  \  - openapi/confluent-the-data-streaming-platform-cloud-apis-openapi.yml\ndocs: https://docs.confluent.io/cloud/current/api.html#authentication\ndocs_notes:\n  api_key_categories:\n  - name: Cloud API key\n    grants: The Confluent Cloud Management APIs — provisioning and metrics integrations.\n  - name: Resource-specific API key\n    grants: One Confluent Kafka cluster, Schema Registry cluster, ksqlDB cluster or Flink region.\n  transport: HTTP Basic — API key ID as username, secret as password.\n  oauth: OAuth 2.0 client credentials against https://api.confluent.cloud/sts/v1/oauth2/token (Confluent\n    STS), or a token from an external IdP registered as an identity provider.\n  workload_identity: iam/v2 identity-providers and identity-pools support OIDC federation, so a workload\n    can exchange an external IdP token rather than holding a long-lived key.\n  key_management: Keys are created and rotated with createIamV2ApiKey / deleteIamV2ApiKey or the confluent\n    CLI. The secret\
  \ is returned once at creation and cannot be retrieved again.\n  mcp: 'The managed MCP servers reuse the same credentials, base64-encoded into an Authorization: Basic\n    header. Global API keys work on both managed servers; Cloud API keys on the global server only; Flink\n    API keys on the regional server only.'\n  scopes: Only the partner OAuth scheme declares scopes (partner:describe / create / alter / delete).\n    Everything else is authorized by RBAC role bindings, not by token scope.\n  source:\n  - https://docs.confluent.io/cloud/current/api.html\n  - https://docs.confluent.io/cloud/current/security/authenticate/workload-identities/service-accounts/api-keys/overview.html\n  - https://docs.confluent.io/cloud/current/ai/ai-tools/managed-mcp-server.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent-the-data-streaming-platform/refs/heads/main/authentication/confluent-the-data-streaming-platform-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Apache Flink
- Apache Kafka
- Confluent Cloud
- Connectors
- Data Streaming
- Event Streaming
- Kafka Connect
- ksqlDB
- Real-Time Data
- REST
- Schema Registry
- Stream Processing
---
