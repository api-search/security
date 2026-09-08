---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dagger-graphql-api-openapi.yml
  format: yaml
  label: Dagger GraphQL API
  slug: dagger-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagger/refs/heads/main/openapi/dagger-graphql-api-openapi.yml
auth_types:
- http
- oidc
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dagger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dagger secures its APIs with http and oidc across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dagger
provider_slug: dagger
scheme_count: 3
schemes:
- credential_source: DAGGER_SESSION_TOKEN environment variable, set per session by `dagger run`
  description: HTTP Basic auth where the username is the value of the DAGGER_SESSION_TOKEN environment variable and the password is empty.
  docs_quote: '"Dagger protects the exposed API with an HTTP Basic authentication token which can be retrieved from the DAGGER_SESSION_TOKEN variable. Treat the DAGGER_SESSION_TOKEN value as you would any other sensitive credential."'
  example: "curl -s \\\n  -u $DAGGER_SESSION_TOKEN: \\\n  -H \"content-type:application/json\" \\\n  -d @- \\\n  http://127.0.0.1:$DAGGER_SESSION_PORT/query"
  lifetime: single session
  name: SessionTokenBasic
  rotation: automatic — a new token is minted for every session
  scheme: basic
  sources:
  - openapi/dagger-graphql-api-openapi.yml
  - https://docs.dagger.io/0.21/getting-started/api/http/
  surface: Dagger Engine GraphQL API
  type: http
- credential_source: DAGGER_CLOUD_TOKEN environment variable
  description: Dagger Cloud telemetry upload is authenticated with a token supplied in the DAGGER_CLOUD_TOKEN environment variable. Documented for Kubernetes as a secret named `dagger-cloud` holding that value.
  in: environment
  name: DaggerCloudToken
  sources:
  - https://docs.dagger.io/configuration/cloud/
  surface: Dagger Cloud
  type: apiKey
- artifact: well-known/dagger-openid-configuration.json
  description: api.dagger.cloud publishes an OIDC discovery document. It advertises id_token issuance only — issuer https://api.dagger.cloud, jwks_uri https://api.dagger.cloud/jwks (200, one RS256 RSA key), response_types_supported [id_token], subject_types_supported [public] — with no authorization_endpoint, token_endpoint or scopes_supported. It is an identity-token issuer for verifying Dagger Cloud workload identity, not an OP an application runs an authorization code flow against.
  discovery: https://api.dagger.cloud/.well-known/openid-configuration
  http_status: 200
  name: DaggerCloudOIDC
  probed: '2026-09-07'
  surface: Dagger Cloud (api.dagger.cloud)
  type: openIdConnect
slug: dagger-authentication
source_filename: dagger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://docs.dagger.io/0.21/getting-started/api/http/ (session endpoint, token,\n  Basic auth, verbatim curl example), https://docs.dagger.io/configuration/cloud/\n  (DAGGER_CLOUD_TOKEN), the OIDC discovery document probed at\n  https://api.dagger.cloud/.well-known/openid-configuration and saved at\n  well-known/dagger-openid-configuration.json, and the securitySchemes block of\n  openapi/dagger-graphql-api-openapi.yml\ndocs: https://docs.dagger.io/0.21/getting-started/api/http/\nsummary:\n  types:\n  - http\n  - oidc\n  oauth2: false\n  api_key: false\n  mtls: false\nschemes:\n- name: SessionTokenBasic\n  type: http\n  scheme: basic\n  surface: Dagger Engine GraphQL API\n  description: >-\n    HTTP Basic auth where the username is the value of the DAGGER_SESSION_TOKEN\n    environment variable and the password is empty.\n  credential_source: DAGGER_SESSION_TOKEN environment variable, set per session by `dagger run`\n\
  \  lifetime: single session\n  rotation: automatic — a new token is minted for every session\n  docs_quote: >-\n    \"Dagger protects the exposed API with an HTTP Basic authentication token which\n    can be retrieved from the DAGGER_SESSION_TOKEN variable. Treat the\n    DAGGER_SESSION_TOKEN value as you would any other sensitive credential.\"\n  example: |-\n    curl -s \\\n      -u $DAGGER_SESSION_TOKEN: \\\n      -H \"content-type:application/json\" \\\n      -d @- \\\n      http://127.0.0.1:$DAGGER_SESSION_PORT/query\n  sources:\n  - openapi/dagger-graphql-api-openapi.yml\n  - https://docs.dagger.io/0.21/getting-started/api/http/\n- name: DaggerCloudToken\n  type: apiKey\n  in: environment\n  surface: Dagger Cloud\n  description: >-\n    Dagger Cloud telemetry upload is authenticated with a token supplied in the\n    DAGGER_CLOUD_TOKEN environment variable. Documented for Kubernetes as a\n    secret named `dagger-cloud` holding that value.\n  credential_source: DAGGER_CLOUD_TOKEN\
  \ environment variable\n  sources:\n  - https://docs.dagger.io/configuration/cloud/\n- name: DaggerCloudOIDC\n  type: openIdConnect\n  surface: Dagger Cloud (api.dagger.cloud)\n  description: >-\n    api.dagger.cloud publishes an OIDC discovery document. It advertises id_token\n    issuance only — issuer https://api.dagger.cloud, jwks_uri\n    https://api.dagger.cloud/jwks (200, one RS256 RSA key),\n    response_types_supported [id_token], subject_types_supported [public] — with\n    no authorization_endpoint, token_endpoint or scopes_supported. It is an\n    identity-token issuer for verifying Dagger Cloud workload identity, not an\n    OP an application runs an authorization code flow against.\n  discovery: https://api.dagger.cloud/.well-known/openid-configuration\n  probed: '2026-09-07'\n  http_status: 200\n  artifact: well-known/dagger-openid-configuration.json\nscopes:\n  published: false\n  note: >-\n    No OAuth 2.0 scopes exist. There is no oauth2 securityScheme in the contract\n\
  \    and /.well-known/oauth-authorization-server returns 404 on every Dagger host\n    probed. Authorization on the engine is all-or-nothing per session; the real\n    access control is the sandbox — a function reaches only the Directory,\n    Socket, Service and Secret values explicitly passed to it\n    (https://docs.dagger.io/features/security/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagger/refs/heads/main/authentication/dagger-authentication.yml
summary_line: http/oidc · 3 schemes
tags:
- Build Automation
- BuildKit
- CI/CD
- Containers
- DAG
- Daggerverse
- DevOps
- GraphQL
- Modules
- OCI
- Open-Source
- Pipelines
- Programmable Pipelines
- SDK
---
