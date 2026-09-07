---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudbees-unify-openapi.yml
  format: yaml
  label: CloudBees Unify Platform API
  slug: unify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-unify-openapi.yml
- filename: cloudbees-computer-api-openapi.yml
  format: yaml
  label: CloudBees Computer API
  slug: cloudbees-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-computer-api-openapi.yml
- filename: cloudbees-createitem-api-openapi.yml
  format: yaml
  label: CloudBees CreateItem API
  slug: cloudbees-createitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-createitem-api-openapi.yml
- filename: cloudbees-job-api-openapi.yml
  format: yaml
  label: CloudBees Job API
  slug: cloudbees-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-job-api-openapi.yml
- filename: cloudbees-json-api-openapi.yml
  format: yaml
  label: CloudBees Json API
  slug: cloudbees-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-json-api-openapi.yml
- filename: cloudbees-python-api-openapi.yml
  format: yaml
  label: CloudBees Python API
  slug: cloudbees-python-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-python-api-openapi.yml
- filename: cloudbees-queue-api-openapi.yml
  format: yaml
  label: CloudBees Queue API
  slug: cloudbees-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-queue-api-openapi.yml
- filename: cloudbees-xml-api-openapi.yml
  format: yaml
  label: CloudBees Xml API
  slug: cloudbees-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-xml-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloudbees Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudBees secures its APIs with apiKey, http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CloudBees
provider_slug: cloudbees
scheme_count: 2
schemes:
- description: Jenkins username + API token
  docs: https://docs.cloudbees.com/docs/cloudbees-ci-api/latest/api-authentication
  header: 'Authorization: Basic base64(<username>:<api_token>)'
  name: basicAuth
  note: CloudBees CI API tokens are generated in the UI, can be revoked at any time, and work interchangeably across the REST API and the Jenkins CLI (-auth username:token).
  scheme: basic
  sources:
  - openapi/cloudbees-computer-api-openapi.yml
  - openapi/cloudbees-createitem-api-openapi.yml
  - openapi/cloudbees-job-api-openapi.yml
  - openapi/cloudbees-json-api-openapi.yml
  - openapi/cloudbees-python-api-openapi.yml
  - openapi/cloudbees-queue-api-openapi.yml
  - openapi/cloudbees-xml-api-openapi.yml
  surface: CloudBees CI (Jenkins-compatible) controllers — customer-operated
  type: http
- description: CloudBees Unify API access token or personal access token
  docs: https://docs.cloudbees.com/docs/cloudbees-platform/latest/workflows/personal-access-token
  header: 'Authorization: Bearer <personal_access_token>'
  name: BearerAuth
  note: PATs are created in the CloudBees Unify UI under the user profile and inherit that user's permissions — there is no scope narrowing on the REST surface.
  scheme: bearer
  sources:
  - openapi/cloudbees-unify-beta-openapi.yml
  - openapi/cloudbees-unify-openapi.yml
  surface: CloudBees Unify Public API (https://api.cloudbees.io)
  token_types:
  - personal access token (PAT)
  - CloudBees Unify API access token
  type: http
slug: cloudbees-authentication
source_filename: cloudbees-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/cloudbees-computer-api-openapi.yml, openapi/cloudbees-createitem-api-openapi.yml, openapi/cloudbees-job-api-openapi.yml,\n  openapi/cloudbees-json-api-openapi.yml, openapi/cloudbees-python-api-openapi.yml, openapi/cloudbees-queue-api-openapi.yml,\n  openapi/cloudbees-unify-beta-openapi.yml, openapi/cloudbees-unify-openapi.yml, openapi/cloudbees-xml-api-openapi.yml;\n  upgraded from the CloudBees docs (personal access tokens, CloudBees CI API authentication) and live probes of\n  the OAuth/OIDC discovery documents on 2026-09-05\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  note: http/bearer and http/basic are what the harvested OpenAPI documents declare; oauth2, openIdConnect and apiKey\n    come from the additional surfaces below, which have no published OpenAPI.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Jenkins username + API token\n  sources:\n  - openapi/cloudbees-computer-api-openapi.yml\n\
  \  - openapi/cloudbees-createitem-api-openapi.yml\n  - openapi/cloudbees-job-api-openapi.yml\n  - openapi/cloudbees-json-api-openapi.yml\n  - openapi/cloudbees-python-api-openapi.yml\n  - openapi/cloudbees-queue-api-openapi.yml\n  - openapi/cloudbees-xml-api-openapi.yml\n  surface: CloudBees CI (Jenkins-compatible) controllers — customer-operated\n  header: 'Authorization: Basic base64(<username>:<api_token>)'\n  docs: https://docs.cloudbees.com/docs/cloudbees-ci-api/latest/api-authentication\n  note: CloudBees CI API tokens are generated in the UI, can be revoked at any time, and work interchangeably across\n    the REST API and the Jenkins CLI (-auth username:token).\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: CloudBees Unify API access token or personal access token\n  sources:\n  - openapi/cloudbees-unify-beta-openapi.yml\n  - openapi/cloudbees-unify-openapi.yml\n  surface: CloudBees Unify Public API (https://api.cloudbees.io)\n  header: 'Authorization: Bearer\
  \ <personal_access_token>'\n  token_types:\n  - personal access token (PAT)\n  - CloudBees Unify API access token\n  docs: https://docs.cloudbees.com/docs/cloudbees-platform/latest/workflows/personal-access-token\n  note: PATs are created in the CloudBees Unify UI under the user profile and inherit that user's permissions —\n    there is no scope narrowing on the REST surface.\ndocs: https://docs.cloudbees.com/docs/cloudbees-platform/latest/workflows/personal-access-token\nadditional_surfaces:\n- name: CloudBees Unify MCP Server\n  endpoint: https://mcp.cloudbees.io/v1/mcp\n  type: oauth2\n  flow: authorizationCode\n  authorization_servers:\n  - https://id.cloudbees.io/realms/cloudbees\n  scopes:\n  - openid\n  - profile\n  - email\n  - mcp:unify:connect\n  discovery: https://mcp.cloudbees.io/.well-known/oauth-protected-resource\n  evidence: RFC 9728 protected-resource document + WWW-Authenticate Bearer challenge observed 2026-09-05\n  cross_ref: scopes/cloudbees-scopes.yml\n- name: CloudBees\
  \ Feature Management REST API\n  endpoint: https://x-api.rollout.io/public-api\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <API_TOKEN>'\n  docs: https://docs.cloudbees.com/docs/cloudbees-feature-management-rest-api/latest/introduction\n- name: CloudBees CD/RO REST API\n  endpoint: https://<cd-server>/rest/v1.0/\n  type: apiKey\n  in: header\n  parameter: sessionid\n  docs: https://docs.cloudbees.com/docs/cloudbees-cd-api-rest/latest/\n  note: Session id from `ectool login`, or a user-generated API token, passed as a sessionid header.\n- name: CloudBees Unify workload identity (OIDC issuer)\n  issuer: https://api.cloudbees.io\n  type: openIdConnect\n  discovery: https://api.cloudbees.io/.well-known/openid-configuration\n  response_types_supported:\n  - id_token\n  claims:\n  - sub\n  - aud\n  - exp\n  - iat\n  - iss\n  - jti\n  - nbf\n  - ref\n  - repository\n  - run_id\n  - run_number\n  - run_attempt\n  note: Issues id_tokens identifying a workflow RUN, for federating\
  \ CloudBees Unify workflows into cloud providers\n    without static credentials. Not a user-facing login.\n  file: well-known/cloudbees-api-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/authentication/cloudbees-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 2 schemes
tags:
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Feature Flags
- Feature Management
- Jenkins
- Release Orchestration
- Software Delivery
---
