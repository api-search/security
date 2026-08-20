---
api_key_in:
- header
api_specs:
- filename: stacklok-clients-api-openapi.yml
  format: yaml
  label: Stacklok clients API
  slug: stacklok-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-clients-api-openapi.yml
- filename: stacklok-discovery-api-openapi.yml
  format: yaml
  label: Stacklok discovery API
  slug: stacklok-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-discovery-api-openapi.yml
- filename: stacklok-groups-api-openapi.yml
  format: yaml
  label: Stacklok groups API
  slug: stacklok-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-groups-api-openapi.yml
- filename: stacklok-logs-api-openapi.yml
  format: yaml
  label: Stacklok logs API
  slug: stacklok-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-logs-api-openapi.yml
- filename: stacklok-registry-api-openapi.yml
  format: yaml
  label: Stacklok registry API
  slug: stacklok-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-registry-api-openapi.yml
- filename: stacklok-registry-servers-api-openapi.yml
  format: yaml
  label: Stacklok registry-servers API
  slug: stacklok-registry-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-registry-servers-api-openapi.yml
- filename: stacklok-registry-skills-api-openapi.yml
  format: yaml
  label: Stacklok registry-skills API
  slug: stacklok-registry-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-registry-skills-api-openapi.yml
- filename: stacklok-secrets-api-openapi.yml
  format: yaml
  label: Stacklok secrets API
  slug: stacklok-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-secrets-api-openapi.yml
- filename: stacklok-skills-api-openapi.yml
  format: yaml
  label: Stacklok skills API
  slug: stacklok-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-skills-api-openapi.yml
- filename: stacklok-system-api-openapi.yml
  format: yaml
  label: Stacklok system API
  slug: stacklok-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-system-api-openapi.yml
- filename: stacklok-v1-api-openapi.yml
  format: yaml
  label: Stacklok v1 API
  slug: stacklok-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-v1-api-openapi.yml
- filename: stacklok-version-api-openapi.yml
  format: yaml
  label: Stacklok version API
  slug: stacklok-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-version-api-openapi.yml
- filename: stacklok-workloads-api-openapi.yml
  format: yaml
  label: Stacklok workloads API
  slug: stacklok-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-workloads-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Stacklok Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stacklok secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stacklok
provider_slug: stacklok
scheme_count: 1
schemes:
- description: 'OAuth 2.0 / OIDC Bearer token authentication. Format: "Bearer {token}"'
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/stacklok-registry-api-openapi.yml
  type: apiKey
slug: stacklok-authentication
source_filename: stacklok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stacklok-registry-api-openapi.yml, openapi/stacklok-toolhive-api-openapi.yml\ndocs: https://docs.stacklok.com\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  detail: >-\n    The ToolHive Registry API requires OAuth 2.0 / OIDC Bearer access tokens in the\n    Authorization header (Authorization: Bearer {token}). OAuth discovery metadata is\n    published at /.well-known/oauth-protected-resource (RFC 9728). Enterprise deployments\n    integrate external identity providers (Okta, Auth0, Microsoft Entra ID) for OIDC\n    sign-in; an anonymous mode is available for local development. The local ToolHive\n    control API (thv serve) does not declare an in-spec security scheme.\nschemes:\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'OAuth 2.0 / OIDC Bearer token authentication. Format: \"Bearer {token}\"'\n  sources:\n  - openapi/stacklok-registry-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/authentication/stacklok-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Open-Source
---
