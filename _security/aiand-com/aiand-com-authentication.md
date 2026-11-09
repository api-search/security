---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aiand-com-files-api-openapi.yml
  format: yaml
  label: ai& Files API
  slug: aiand-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiand-com/openapi/aiand-com-files-api-openapi.yml
- filename: aiand-com-logs-api-openapi.yml
  format: yaml
  label: ai& Logs API
  slug: aiand-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiand-com/openapi/aiand-com-logs-api-openapi.yml
- filename: aiand-com-openai-api-openapi.yml
  format: yaml
  label: ai& Openai API
  slug: aiand-com-openai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiand-com/openapi/aiand-com-openai-api-openapi.yml
- filename: aiand-com-uploads-api-openapi.yml
  format: yaml
  label: ai& Uploads API
  slug: aiand-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiand-com/openapi/aiand-com-uploads-api-openapi.yml
- filename: aiand-com-videos-api-openapi.yml
  format: yaml
  label: ai& Videos API
  slug: aiand-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiand-com/openapi/aiand-com-videos-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aiand Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ai& declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ai&
provider_slug: aiand-com
scheme_count: 3
schemes:
- description: API Key (recommended) passed as Bearer token.
  in: header
  name: Authorization
  type: apiKey
- bearerFormat: JWT
  description: Session authentication via JWT stored in httpOnly cookies.
  scheme: bearer
  type: http
- description: Enterprise SSO via SAML (Okta, Entra ID, etc.)
  type: saml
slug: aiand-com-authentication
source_filename: aiand-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://docs.aiand.com/authentication/\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: API Key (recommended) passed as Bearer token.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Session authentication via JWT stored in httpOnly cookies.\n  - type: saml\n    description: Enterprise SSO via SAML (Okta, Entra ID, etc.)\n"
source_yaml_url: https://artifacts.apis.io/aiand-com/authentication/aiand-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Japan
- Inference
- Machine Learning
- Startups
---
