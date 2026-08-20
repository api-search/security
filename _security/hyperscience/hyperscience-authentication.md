---
api_key_in: []
api_specs:
- filename: hyperscience-audit-logs-api-openapi.yml
  format: yaml
  label: Hyperscience Audit Logs API
  slug: hyperscience-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-audit-logs-api-openapi.yml
- filename: hyperscience-cases-api-openapi.yml
  format: yaml
  label: Hyperscience Cases API
  slug: hyperscience-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-cases-api-openapi.yml
- filename: hyperscience-documents-api-openapi.yml
  format: yaml
  label: Hyperscience Documents API
  slug: hyperscience-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-documents-api-openapi.yml
- filename: hyperscience-flow-runs-api-openapi.yml
  format: yaml
  label: Hyperscience Flow Runs API
  slug: hyperscience-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flow-runs-api-openapi.yml
- filename: hyperscience-flows-api-openapi.yml
  format: yaml
  label: Hyperscience Flows API
  slug: hyperscience-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flows-api-openapi.yml
- filename: hyperscience-layouts-api-openapi.yml
  format: yaml
  label: Hyperscience Layouts API
  slug: hyperscience-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-layouts-api-openapi.yml
- filename: hyperscience-pages-api-openapi.yml
  format: yaml
  label: Hyperscience Pages API
  slug: hyperscience-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-pages-api-openapi.yml
- filename: hyperscience-submissions-api-openapi.yml
  format: yaml
  label: Hyperscience Submissions API
  slug: hyperscience-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-submissions-api-openapi.yml
- filename: hyperscience-version-api-openapi.yml
  format: yaml
  label: Hyperscience Version API
  slug: hyperscience-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-version-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hyperscience Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hyperscience secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hyperscience
provider_slug: hyperscience
scheme_count: 1
schemes:
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  sources:
  - openapi/hyperscience-openapi.yml
  type: oauth2
slug: hyperscience-authentication
source_filename: hyperscience-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperscience-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n  sources:\n  - openapi/hyperscience-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/authentication/hyperscience-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Document AI
- IDP
- Enterprise
- Automation
- GenAI
- FedRAMP
---
