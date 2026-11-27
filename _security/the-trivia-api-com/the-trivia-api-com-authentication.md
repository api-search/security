---
anonymous_access: false
api_key_in: []
api_specs:
- filename: the-trivia-api-com-meta-api-openapi.yml
  format: yaml
  label: The Trivia API Meta API
  slug: the-trivia-api-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-meta-api-openapi.yml
- filename: the-trivia-api-com-questions-api-openapi.yml
  format: yaml
  label: The Trivia API Questions API
  slug: the-trivia-api-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-questions-api-openapi.yml
- filename: the-trivia-api-com-quizzes-api-openapi.yml
  format: yaml
  label: The Trivia API Quizzes API
  slug: the-trivia-api-com-quizzes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-quizzes-api-openapi.yml
- filename: the-trivia-api-com-sessions-api-openapi.yml
  format: yaml
  label: The Trivia API Sessions API
  slug: the-trivia-api-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-trivia-api-com/openapi/the-trivia-api-com-sessions-api-openapi.yml
auth_types: []
description: Authentication with an API key
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: The Trivia API Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Trivia API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Trivia API
provider_slug: the-trivia-api-com
scheme_count: 1
schemes:
- evidence: Send your API key in the X-API-Key header to use other languages, typed answers, image questions, sessions and more.
  header: X-API-Key
  how_to_obtain: Keys come with a subscription; obtain your key from your account page after signing in.
  location: header
  name: X-API-Key
  type: apiKey
slug: the-trivia-api-com-authentication
source_filename: the-trivia-api-com-authentication.yml
source_heading: Authentication Profile
source_url: https://the-trivia-api.com/docs/authentication.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://the-trivia-api.com/docs/authentication.md\nsources:\n- https://the-trivia-api.com/docs/authentication.md\n- https://the-trivia-api.com/docs/authentication/\n- https://the-trivia-api.com/docs/authentication/\n- https://the-trivia-api.com/docs.md\ndescription: Authentication with an API key\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send your API key in the X-API-Key header to use other languages, typed answers, image questions, sessions and more.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Keys come with a subscription; obtain your key from your account page after signing in.\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://the-trivia-api.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/the-trivia-api-com/authentication/the-trivia-api-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Trivia
- JSON
- Questions
---
