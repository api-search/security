---
anonymous_access: false
api_key_in: []
api_specs:
- filename: classifier-dev-account-api-openapi.yml
  format: yaml
  label: classifier-dev Account API
  slug: classifier-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-account-api-openapi.yml
- filename: classifier-dev-classifier-dev-api-openapi.yml
  format: yaml
  label: classifier-dev Classifier.dev API
  slug: classifier-dev-classifier-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classifier-dev-api-openapi.yml
- filename: classifier-dev-classify-api-openapi.yml
  format: yaml
  label: classifier-dev Classify API
  slug: classifier-dev-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classify-api-openapi.yml
- filename: classifier-dev-docs-api-openapi.yml
  format: yaml
  label: classifier-dev Docs API
  slug: classifier-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-docs-api-openapi.yml
- filename: classifier-dev-feedback-api-openapi.yml
  format: yaml
  label: classifier-dev Feedback API
  slug: classifier-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-feedback-api-openapi.yml
- filename: classifier-dev-subscribe-api-openapi.yml
  format: yaml
  label: classifier-dev Subscribe API
  slug: classifier-dev-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-subscribe-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Classifier Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: classifier-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: classifier-dev
provider_slug: classifier-dev
scheme_count: 2
schemes:
- description: Workspace API key (classifier_agent_...) required for account reads; optional on classification.
  name: accountKey
  scheme: bearer
  type: http
- description: Optional partner key for classification.
  name: partnerKey
  scheme: bearer
  type: http
slug: classifier-dev-authentication
source_filename: classifier-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://classifier.dev/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    name: accountKey\n    description: Workspace API key (classifier_agent_...) required for account reads; optional on classification.\n  - type: http\n    scheme: bearer\n    name: partnerKey\n    description: Optional partner key for classification.\n"
source_yaml_url: https://artifacts.apis.io/classifier-dev/authentication/classifier-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Machine Learning
- NLP
- Classification
- API
- OpenAPI
---
