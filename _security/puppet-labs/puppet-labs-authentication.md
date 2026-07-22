---
api_key_in:
- header
api_specs:
- filename: puppet-labs-forge-openapi-original.json
  format: json
  label: Puppet Forge v3 API
  slug: puppet-forge-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puppet-labs/refs/heads/main/openapi/puppet-labs-forge-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Puppet Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Puppet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Puppet
provider_slug: puppet-labs
scheme_count: 1
schemes:
- description: 'Some of the Forge API endpoints require authentication in the form of a user API key. API keys may be created and revoked from a user''s profile on the [Forge website](https://forge.puppet.com), where other profile details are managed.


    To perform actions that require API key authentication, the key must be present in an `Authorization` header with the request. The header should be formatted as:


    `'
  in: header
  name: ApiKeyAuth
  parameter: 'Authorization: Bearer <api_key>'
  sources:
  - openapi/puppet-labs-forge-openapi-original.json
  type: apiKey
slug: puppet-labs-authentication
source_filename: puppet-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/puppet-labs-forge-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: 'Authorization: Bearer <api_key>'\n  description: |-\n    Some of the Forge API endpoints require authentication in the form of a user API key. API keys may be created and revoked from a user's profile on the [Forge website](https://forge.puppet.com), where other profile details are managed.\n\n    To perform actions that require API key authentication, the key must be present in an `Authorization` header with the request. The header should be formatted as:\n\n    `\n  sources:\n  - openapi/puppet-labs-forge-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puppet-labs/refs/heads/main/authentication/puppet-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Infrastructure Automation
- Configuration Management
- DevOps
- Module Registry
- Compliance
---
