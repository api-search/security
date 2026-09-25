---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: 4paradigm-account-api-openapi.yml
  format: yaml
  label: 4Paradigm Account API
  slug: 4paradigm-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-account-api-openapi.yml
- filename: 4paradigm-applications-api-openapi.yml
  format: yaml
  label: 4Paradigm Applications API
  slug: 4paradigm-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-applications-api-openapi.yml
- filename: 4paradigm-competition-api-openapi.yml
  format: yaml
  label: 4Paradigm Competition API
  slug: 4paradigm-competition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-competition-api-openapi.yml
- filename: 4paradigm-computeunit-api-openapi.yml
  format: yaml
  label: 4Paradigm Computeunit API
  slug: 4paradigm-computeunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-computeunit-api-openapi.yml
- filename: 4paradigm-computing-resource-api-openapi.yml
  format: yaml
  label: 4Paradigm Computing Resource API
  slug: 4paradigm-computing-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-computing-resource-api-openapi.yml
- filename: 4paradigm-environments-api-openapi.yml
  format: yaml
  label: 4Paradigm Environments API
  slug: 4paradigm-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-environments-api-openapi.yml
- filename: 4paradigm-finished-api-openapi.yml
  format: yaml
  label: 4Paradigm Finished API
  slug: 4paradigm-finished-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-finished-api-openapi.yml
- filename: 4paradigm-images-api-openapi.yml
  format: yaml
  label: 4Paradigm Images API
  slug: 4paradigm-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-images-api-openapi.yml
- filename: 4paradigm-logs-api-openapi.yml
  format: yaml
  label: 4Paradigm Logs API
  slug: 4paradigm-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-logs-api-openapi.yml
- filename: 4paradigm-releases-api-openapi.yml
  format: yaml
  label: 4Paradigm Releases API
  slug: 4paradigm-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-releases-api-openapi.yml
- filename: 4paradigm-storage-api-openapi.yml
  format: yaml
  label: 4Paradigm Storage API
  slug: 4paradigm-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-storage-api-openapi.yml
- filename: 4paradigm-users-api-openapi.yml
  format: yaml
  label: 4Paradigm Users API
  slug: 4paradigm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-users-api-openapi.yml
- filename: 4paradigm-app-store-api-openapi.yml
  format: yaml
  label: 4Paradigm App Store API
  slug: 4paradigm-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-app-store-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
- none
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: 4Paradigm Authentication
name_suffix: Authentication
oauth_flows: []
overview: 4Paradigm secures its APIs with apiKey, openIdConnect, and none across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 4Paradigm
provider_slug: 4paradigm
scheme_count: 6
schemes:
- in: header
  name: ApiKeyAuth
  note: Declared as a raw apiKey in the Authorization header — no scheme prefix (no `Bearer`, no `ApiKey`) is specified by the contract, and no key format, rotation or issuance is documented.
  parameter: Authorization
  sources:
  - openapi/4paradigm-openaios-billing.yaml
  - openapi/4paradigm-openaios-platform.yaml
  surface: OpenAIOS-Platform, OpenAIOS Billing
  type: apiKey
- name: OpenID
  note: The discovery document is relative, so it resolves against the operator's own deployment. No 4Paradigm-hosted OIDC issuer exists; probed 2026-09-05, every 4paradigm.com host returns a 404 or an HTML catch-all for /.well-known/openid-configuration.
  openIdConnectUrl: /.well-known/openid-configuration
  scopes_requested:
  - openid
  - email
  - profile
  sources:
  - openapi/4paradigm-openaios-platform.yaml
  surface: OpenAIOS-Platform
  type: openIdConnect
- detail: Introduced in 0.8.5 and made an explicit alpha in 0.9.0. Off unless every client and server is started with --skip_grant_tables=false. Until then the cluster accepts the root user with an EMPTY password, and CREATE USER / ALTER USER / DELETE USER are rejected. Credentials are set with SQL (`alter user root set options (password='...')`), and the APIServer and TaskManager must themselves be reconfigured with --user/--password because they connect as clients.
  docs: https://openmldb.ai/docs/en/main/deploy/auth.html
  name: OpenMLDB cluster authentication
  status: alpha, disabled by default
  surface: OpenMLDB (SDKs, CLI, APIServer, TaskManager)
  type: username-password
- detail: Separate from cluster authentication. Configured as zookeeper.cert=user:passwd (TaskManager), --zk_cert=user:passwd (servers and CLI), SdkOption.setZkCert(...) (Java) or zkCert= (Python), and it may be passed inside a JDBC URL — which puts a credential in a connection string.
  docs: https://openmldb.ai/docs/en/main/deploy/auth.html
  name: ZooKeeper credentials
  status: available since 0.8.4
  surface: OpenMLDB cluster coordination
  type: username-password
- detail: No auth is declared in any driver.yaml. The security model is the loopback bind plus the private network the robot sits on. Identity, pairing and signed requests exist only for robot-to-robot peer delegation, not for the tool surface an agent calls.
  name: PhanthyMotus driver MCP endpoints
  sources:
  - mcp/4paradigm-mcp.yml
  surface: http://localhost:<port>/mcp, 16 driver bundles
  type: none
- detail: Live, public and unauthenticated — /api/model, /api/model-category, /api/solutions, /api/highlights/latest and /api/top-banners all returned 200 application/json to an anonymous request on 2026-09-05. Read-only catalogue content; no credential is offered or required.
  method: probed
  name: Sage App Store catalogue API
  surface: https://apps.4paradigm.com/api
  type: none
slug: 4paradigm-authentication
source_filename: 4paradigm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  derived from openapi/4paradigm-openaios-billing.yaml and openapi/4paradigm-openaios-platform.yaml,\n  then upgraded from 4Paradigm's own documentation at https://openmldb.ai/docs/en/main/deploy/auth.html\n  and https://github.com/4paradigm/phanthymotus#readme (fetched 2026-09-05), plus a live unauthenticated\n  probe of https://apps.4paradigm.com/api/ on 2026-09-05\ndocs: https://openmldb.ai/docs/en/main/deploy/auth.html\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  - none\n  api_key_in:\n  - header\n  note: >-\n    4Paradigm issues no credentials for anything. Every scheme below is enforced by software you run\n    yourself, so \"authentication\" here means what the shipped default is — and the shipped defaults are\n    weak: OpenMLDB runs as root with an empty password unless you turn authentication on, PhanthyMotus\n    driver MCP endpoints declare no auth at all, and the one publicly reachable surface is open.\n\
  schemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  surface: OpenAIOS-Platform, OpenAIOS Billing\n  sources:\n  - openapi/4paradigm-openaios-billing.yaml\n  - openapi/4paradigm-openaios-platform.yaml\n  note: >-\n    Declared as a raw apiKey in the Authorization header — no scheme prefix (no `Bearer`, no `ApiKey`)\n    is specified by the contract, and no key format, rotation or issuance is documented.\n- name: OpenID\n  type: openIdConnect\n  openIdConnectUrl: /.well-known/openid-configuration\n  scopes_requested: [openid, email, profile]\n  surface: OpenAIOS-Platform\n  sources:\n  - openapi/4paradigm-openaios-platform.yaml\n  note: >-\n    The discovery document is relative, so it resolves against the operator's own deployment. No\n    4Paradigm-hosted OIDC issuer exists; probed 2026-09-05, every 4paradigm.com host returns a 404 or\n    an HTML catch-all for /.well-known/openid-configuration.\n- name: OpenMLDB cluster authentication\n  type: username-password\n\
  \  surface: OpenMLDB (SDKs, CLI, APIServer, TaskManager)\n  status: alpha, disabled by default\n  docs: https://openmldb.ai/docs/en/main/deploy/auth.html\n  detail: >-\n    Introduced in 0.8.5 and made an explicit alpha in 0.9.0. Off unless every client and server is\n    started with --skip_grant_tables=false. Until then the cluster accepts the root user with an EMPTY\n    password, and CREATE USER / ALTER USER / DELETE USER are rejected. Credentials are set with SQL\n    (`alter user root set options (password='...')`), and the APIServer and TaskManager must\n    themselves be reconfigured with --user/--password because they connect as clients.\n- name: ZooKeeper credentials\n  type: username-password\n  surface: OpenMLDB cluster coordination\n  status: available since 0.8.4\n  docs: https://openmldb.ai/docs/en/main/deploy/auth.html\n  detail: >-\n    Separate from cluster authentication. Configured as zookeeper.cert=user:passwd (TaskManager),\n    --zk_cert=user:passwd (servers and\
  \ CLI), SdkOption.setZkCert(...) (Java) or zkCert= (Python), and\n    it may be passed inside a JDBC URL — which puts a credential in a connection string.\n- name: PhanthyMotus driver MCP endpoints\n  type: none\n  surface: 'http://localhost:<port>/mcp, 16 driver bundles'\n  sources:\n  - mcp/4paradigm-mcp.yml\n  detail: >-\n    No auth is declared in any driver.yaml. The security model is the loopback bind plus the private\n    network the robot sits on. Identity, pairing and signed requests exist only for robot-to-robot peer\n    delegation, not for the tool surface an agent calls.\n- name: Sage App Store catalogue API\n  type: none\n  surface: https://apps.4paradigm.com/api\n  method: probed\n  detail: >-\n    Live, public and unauthenticated — /api/model, /api/model-category, /api/solutions,\n    /api/highlights/latest and /api/top-banners all returned 200 application/json to an anonymous\n    request on 2026-09-05. Read-only catalogue content; no credential is offered or required.\n\
  mtls:\n  supported: false\ntoken_endpoints:\n  published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/authentication/4paradigm-authentication.yml
summary_line: apiKey/openIdConnect/none · 6 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Feature Store
- Database
- Open Source
- MLOps
- Agents
- Robotics
- Kubernetes
---
