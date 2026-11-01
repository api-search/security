---
anonymous_access: false
api_key_in: []
api_specs:
- filename: thehive-ai-task-api-openapi.yml
  format: yaml
  label: Hive Task API
  slug: thehive-ai-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thehive-ai/openapi/thehive-ai-task-api-openapi.yml
auth_types: []
description: Hive V2 API uses a simple API key passed in the HTTP header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Thehive Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hive
provider_slug: thehive-ai
scheme_count: 1
schemes:
- evidence: 'To authenticate requests, include your API key in the HTTP header:'
  header: authorization
  location: header
  name: API Key
  type: apiKey
slug: thehive-ai-authentication
source_filename: thehive-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.thehive.ai/reference/authentication.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.thehive.ai/reference/authentication.md\nsources:\n- https://docs.thehive.ai/reference/authentication.md\n- https://docs.thehive.ai/docs/getting-started.md\n- https://docs.thehive.ai/docs/automl-overview.md\n- https://docs.thehive.ai/docs/moderation-dashboard-quickstart-tutorial.md\ndescription: Hive V2 API uses a simple API key passed in the HTTP header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'To authenticate requests, include your API key in the HTTP header:'\n  location: header\n  header: authorization\nnote: No OAuth2, HTTP basic, bearer, JWT, HMAC, mTLS, or other authentication methods are documented.\ndocs: https://docs.thehive.ai/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/thehive-ai/authentication/thehive-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Machine Learning
- Data Labeling
- Enterprise
---
