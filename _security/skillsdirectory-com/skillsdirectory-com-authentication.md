---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: skillsdirectory-com-categories-api-openapi.yml
  format: yaml
  label: Skills Directory Categories API
  slug: skillsdirectory-com-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-categories-api-openapi.yml
- filename: skillsdirectory-com-registry-api-openapi.yml
  format: yaml
  label: Skills Directory Registry API
  slug: skillsdirectory-com-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-registry-api-openapi.yml
- filename: skillsdirectory-com-scan-api-openapi.yml
  format: yaml
  label: Skills Directory Scan API
  slug: skillsdirectory-com-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-scan-api-openapi.yml
- filename: skillsdirectory-com-skills-api-openapi.yml
  format: yaml
  label: Skills Directory Skills API
  slug: skillsdirectory-com-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-skills-api-openapi.yml
- filename: skillsdirectory-com-stats-api-openapi.yml
  format: yaml
  label: Skills Directory Stats API
  slug: skillsdirectory-com-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/openapi/skillsdirectory-com-stats-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Skillsdirectory Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skills Directory secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skills Directory
provider_slug: skillsdirectory-com
scheme_count: 2
schemes:
- description: 'Authorization: Bearer sk_live_...'
  name: BearerKey
  scheme: bearer
  type: http
- description: Same key as the bearer scheme.
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  type: apiKey
slug: skillsdirectory-com-authentication
source_filename: skillsdirectory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://www.skillsdirectory.com/api-docs\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  bearer: true\n  credential_classes: 1\n  headline: All /api/v1 requests require an sk_live_ API key sent as Authorization Bearer or x-api-key; the Registry API (/api/registry) is public. Live probe returned 401 MISSING_API_KEY with WWW-Authenticate Bearer realm=\"skillsdirectory\".\nschemes:\n- name: BearerKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer sk_live_...'\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Same key as the bearer scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skillsdirectory-com/refs/heads/main/authentication/skillsdirectory-com-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Agent Skills
- AI Agents
- Claude
- Directory
- Security Scanning
---
