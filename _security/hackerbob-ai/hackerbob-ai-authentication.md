---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hackerbob-ai-nlweb-api-openapi.yml
  format: yaml
  label: Hacker Bob NL Web API
  slug: hackerbob-ai-nlweb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-nlweb-api-openapi.yml
- filename: hackerbob-ai-public-cve-records-api-openapi.yml
  format: yaml
  label: Hacker Bob Public CVE records API
  slug: hackerbob-ai-public-cve-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-public-cve-records-api-openapi.yml
- filename: hackerbob-ai-service-api-openapi.yml
  format: yaml
  label: Hacker Bob Service API
  slug: hackerbob-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-service-api-openapi.yml
auth_types: []
description: Authentication methods published for Hacker Bob
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hacker Bob Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hacker Bob declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hacker Bob
provider_slug: hackerbob-ai
scheme_count: 2
schemes:
- evidence: Prefer OAuth 2.1 with PKCE when the host supports protected-resource discovery and dynamic client registration.
  name: OAuth 2.1
  scopes:
  - workspace:read
  - results:read
  - audit:read
  - assets:authorize
  - assessments:prepare
  - assessments:run
  - assessments:cancel
  type: oauth2
- evidence: bearer_methods_supported:["header"]
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: hackerbob-ai-authentication
source_filename: hackerbob-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://hackerbob.ai/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hackerbob.ai/.well-known/oauth-protected-resource\nsources:\n- https://hackerbob.ai/.well-known/oauth-protected-resource\n- https://hackerbob.ai/.well-known/agent-skills/hacker-bob-onboarding.md\ndescription: Authentication methods published for Hacker Bob\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Prefer OAuth 2.1 with PKCE when the host supports protected-resource discovery and dynamic client registration.\n  scopes:\n  - workspace:read\n  - results:read\n  - audit:read\n  - assets:authorize\n  - assessments:prepare\n  - assessments:run\n  - assessments:cancel\n- type: http-bearer\n  name: Bearer\n  evidence: bearer_methods_supported:[\"header\"]\n  location: header\n  header: Authorization\ndocs: https://hackerbob.ai/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/hackerbob-ai/authentication/hackerbob-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Automation
- CVE
- Offensive Security
---
