---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kody-codes-account-api-openapi.yml
  format: yaml
  label: Kody Account API
  slug: kody-codes-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-account-api-openapi.yml
- filename: kody-codes-capability-proxy-api-openapi.yml
  format: yaml
  label: Kody Capability Proxy API
  slug: kody-codes-capability-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-capability-proxy-api-openapi.yml
- filename: kody-codes-community-api-openapi.yml
  format: yaml
  label: Kody Community API
  slug: kody-codes-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-community-api-openapi.yml
- filename: kody-codes-email-api-openapi.yml
  format: yaml
  label: Kody Email API
  slug: kody-codes-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-email-api-openapi.yml
- filename: kody-codes-execute-api-openapi.yml
  format: yaml
  label: Kody Execute API
  slug: kody-codes-execute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-execute-api-openapi.yml
- filename: kody-codes-execution-contexts-api-openapi.yml
  format: yaml
  label: Kody Execution Contexts API
  slug: kody-codes-execution-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-execution-contexts-api-openapi.yml
- filename: kody-codes-files-api-openapi.yml
  format: yaml
  label: Kody Files API
  slug: kody-codes-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-files-api-openapi.yml
- filename: kody-codes-follows-api-openapi.yml
  format: yaml
  label: Kody Follows API
  slug: kody-codes-follows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-follows-api-openapi.yml
- filename: kody-codes-integrations-api-openapi.yml
  format: yaml
  label: Kody Integrations API
  slug: kody-codes-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-integrations-api-openapi.yml
- filename: kody-codes-jobs-api-openapi.yml
  format: yaml
  label: Kody Jobs API
  slug: kody-codes-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-jobs-api-openapi.yml
- filename: kody-codes-mcp-servers-api-openapi.yml
  format: yaml
  label: Kody MCP Servers API
  slug: kody-codes-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-mcp-servers-api-openapi.yml
- filename: kody-codes-memories-api-openapi.yml
  format: yaml
  label: Kody Memories API
  slug: kody-codes-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-memories-api-openapi.yml
- filename: kody-codes-packages-api-openapi.yml
  format: yaml
  label: Kody Packages API
  slug: kody-codes-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-packages-api-openapi.yml
- filename: kody-codes-profiles-api-openapi.yml
  format: yaml
  label: Kody Profiles API
  slug: kody-codes-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-profiles-api-openapi.yml
- filename: kody-codes-repos-api-openapi.yml
  format: yaml
  label: Kody Repos API
  slug: kody-codes-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-repos-api-openapi.yml
- filename: kody-codes-runs-api-openapi.yml
  format: yaml
  label: Kody Runs API
  slug: kody-codes-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-runs-api-openapi.yml
- filename: kody-codes-search-api-openapi.yml
  format: yaml
  label: Kody Search API
  slug: kody-codes-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-search-api-openapi.yml
- filename: kody-codes-secrets-api-openapi.yml
  format: yaml
  label: Kody Secrets API
  slug: kody-codes-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-secrets-api-openapi.yml
- filename: kody-codes-storage-api-openapi.yml
  format: yaml
  label: Kody Storage API
  slug: kody-codes-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-storage-api-openapi.yml
- filename: kody-codes-tokens-api-openapi.yml
  format: yaml
  label: Kody Tokens API
  slug: kody-codes-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-tokens-api-openapi.yml
- filename: kody-codes-webhooks-api-openapi.yml
  format: yaml
  label: Kody Webhooks API
  slug: kody-codes-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kody-codes/openapi/kody-codes-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kody Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kody secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kody
provider_slug: kody-codes
scheme_count: 1
schemes:
- bearerFormat: kody_at_<id>_<secret>
  description: Scoped Kody API token. Each operation lists its required org permission in `x-kody-permission`. Credential scopes narrow that permission.
  name: apiToken
  scheme: bearer
  sources:
  - openapi/kody-codes-openapi.json
  type: http
slug: kody-codes-authentication
source_filename: kody-codes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kody-codes-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  bearerFormat: kody_at_<id>_<secret>\n  description: Scoped Kody API token. Each operation lists its required org permission in `x-kody-permission`.\n    Credential scopes narrow that permission.\n  sources:\n  - openapi/kody-codes-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kody-codes/authentication/kody-codes-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Cloud
- Platform
- Agents
- Collaboration
- Company
---
