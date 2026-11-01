---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mindcloud-api-keys-api-openapi.yml
  format: yaml
  label: MindCloud API Keys API
  slug: mindcloud-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-api-keys-api-openapi.yml
- filename: mindcloud-child-companies-api-openapi.yml
  format: yaml
  label: MindCloud Child Companies API
  slug: mindcloud-child-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-child-companies-api-openapi.yml
- filename: mindcloud-companies-api-openapi.yml
  format: yaml
  label: MindCloud Companies API
  slug: mindcloud-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-companies-api-openapi.yml
- filename: mindcloud-connections-api-openapi.yml
  format: yaml
  label: MindCloud Connections API
  slug: mindcloud-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-connections-api-openapi.yml
- filename: mindcloud-embedded-api-openapi.yml
  format: yaml
  label: MindCloud Embedded API
  slug: mindcloud-embedded-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-embedded-api-openapi.yml
- filename: mindcloud-environments-api-openapi.yml
  format: yaml
  label: MindCloud Environments API
  slug: mindcloud-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-environments-api-openapi.yml
- filename: mindcloud-me-api-openapi.yml
  format: yaml
  label: MindCloud Me API
  slug: mindcloud-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-me-api-openapi.yml
- filename: mindcloud-members-api-openapi.yml
  format: yaml
  label: MindCloud Members API
  slug: mindcloud-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-members-api-openapi.yml
- filename: mindcloud-meta-api-openapi.yml
  format: yaml
  label: MindCloud Meta API
  slug: mindcloud-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-meta-api-openapi.yml
- filename: mindcloud-roles-api-openapi.yml
  format: yaml
  label: MindCloud Roles API
  slug: mindcloud-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-roles-api-openapi.yml
- filename: mindcloud-runs-api-openapi.yml
  format: yaml
  label: MindCloud Runs API
  slug: mindcloud-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-runs-api-openapi.yml
- filename: mindcloud-universal-api-openapi.yml
  format: yaml
  label: MindCloud Universal API
  slug: mindcloud-universal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-universal-api-openapi.yml
- filename: mindcloud-usage-api-openapi.yml
  format: yaml
  label: MindCloud Usage API
  slug: mindcloud-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-usage-api-openapi.yml
- filename: mindcloud-workflows-api-openapi.yml
  format: yaml
  label: MindCloud Workflows API
  slug: mindcloud-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindcloud/openapi/mindcloud-workflows-api-openapi.yml
auth_types: []
description: Authentication schemes for MindCloud API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mindcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: MindCloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MindCloud
provider_slug: mindcloud
scheme_count: 1
schemes:
- evidence: 'Every request needs an API key in the Authorization header:'
  header: Authorization
  location: header
  name: API Key
  type: http-bearer
slug: mindcloud-authentication
source_filename: mindcloud-authentication.yml
source_heading: Authentication Profile
source_url: https://mindcloud.co/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mindcloud.co/.well-known/oauth-protected-resource\nsources:\n- https://mindcloud.co/.well-known/oauth-protected-resource\n- https://mindcloud.co/docs/api/rest/introduction/authentication\n- https://mindcloud.co/docs/cirra/cirra-getting-started/what-is-cirra\ndescription: Authentication schemes for MindCloud API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every request needs an API key in the Authorization header:'\n  location: header\n  header: Authorization\ndocs: https://mindcloud.co/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/mindcloud/authentication/mindcloud-authentication.yml
summary_line: 1 scheme
tags:
- Integration Platform
- Low-Code
- Enterprise Integration
- Workflows
---
