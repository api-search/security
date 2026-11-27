---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emile-wine-api-keys-api-openapi.yml
  format: yaml
  label: Émile API Keys API
  slug: emile-wine-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-api-keys-api-openapi.yml
- filename: emile-wine-auth-api-openapi.yml
  format: yaml
  label: Émile Auth API
  slug: emile-wine-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-auth-api-openapi.yml
- filename: emile-wine-blog-internal-api-openapi.yml
  format: yaml
  label: Émile Blog internal API
  slug: emile-wine-blog-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-blog-internal-api-openapi.yml
- filename: emile-wine-bottles-api-openapi.yml
  format: yaml
  label: Émile Bottles API
  slug: emile-wine-bottles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-bottles-api-openapi.yml
- filename: emile-wine-cellars-api-openapi.yml
  format: yaml
  label: Émile Cellars API
  slug: emile-wine-cellars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-cellars-api-openapi.yml
- filename: emile-wine-dashboard-internal-api-openapi.yml
  format: yaml
  label: Émile Dashboard internal API
  slug: emile-wine-dashboard-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-dashboard-internal-api-openapi.yml
- filename: emile-wine-health-api-openapi.yml
  format: yaml
  label: Émile Health API
  slug: emile-wine-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-health-api-openapi.yml
- filename: emile-wine-legal-api-openapi.yml
  format: yaml
  label: Émile Legal API
  slug: emile-wine-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-legal-api-openapi.yml
- filename: emile-wine-oauth-api-openapi.yml
  format: yaml
  label: Émile OAuth API
  slug: emile-wine-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-oauth-api-openapi.yml
- filename: emile-wine-profile-api-openapi.yml
  format: yaml
  label: Émile Profile API
  slug: emile-wine-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-profile-api-openapi.yml
- filename: emile-wine-rag-api-openapi.yml
  format: yaml
  label: Émile RAG API
  slug: emile-wine-rag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-rag-api-openapi.yml
- filename: emile-wine-rag-internal-api-openapi.yml
  format: yaml
  label: Émile RAG internal API
  slug: emile-wine-rag-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-rag-internal-api-openapi.yml
- filename: emile-wine-recommendations-api-openapi.yml
  format: yaml
  label: Émile Recommendations API
  slug: emile-wine-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-recommendations-api-openapi.yml
- filename: emile-wine-scan-api-openapi.yml
  format: yaml
  label: Émile Scan API
  slug: emile-wine-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-scan-api-openapi.yml
- filename: emile-wine-wines-api-openapi.yml
  format: yaml
  label: Émile Wines API
  slug: emile-wine-wines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emile-wine/openapi/emile-wine-wines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Émile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Émile secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Émile
provider_slug: emile-wine
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/emile-wine-openapi.json
  type: http
slug: emile-wine-authentication
source_filename: emile-wine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/emile-wine-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/emile-wine-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/emile-wine/authentication/emile-wine-authentication.yml
summary_line: http · 1 scheme
tags:
- Wine
- iOS
- Artificial Intelligence
- Privacy
- French
---
