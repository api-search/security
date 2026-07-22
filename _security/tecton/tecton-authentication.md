---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tecton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tecton secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tecton
provider_slug: tecton
scheme_count: 2
schemes:
- bound_to: Service Account
  in: header
  name: ApiKeyAuth
  parameter_name: Authorization
  scheme_value: Tecton-key <API_KEY>
  sources:
  - https://docs.tecton.ai/docs/reading-feature-data/reading-online-features-for-inference-using-the-http-api
  type: apiKey
- audience: Python SDK + CLI (human users)
  mechanism: tecton login (browser SSO via configured identity provider)
  name: InteractiveLogin
  sources:
  - https://docs.tecton.ai/docs/cli
  type: sso
slug: tecton-authentication
source_filename: tecton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tecton.ai/docs/reading-feature-data/reading-online-features-for-inference-using-the-http-api\ndocs: https://docs.tecton.ai/docs/security\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Two authentication surfaces. (1) The FeatureService HTTP API (online inference) is\n    authenticated with a Tecton API key presented in the Authorization header using the\n    \"Tecton-key\" scheme. API keys are issued to Service Accounts and governed by\n    Tecton's access-control (RBAC) model. (2) The Python SDK and `tecton` CLI authenticate\n    interactively via `tecton login` (SSO / identity provider) for humans, and via\n    Service Account API keys for automation/CI.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    scheme_value: \"Tecton-key <API_KEY>\"\n    bound_to: Service Account\n    sources: [https://docs.tecton.ai/docs/reading-feature-data/reading-online-features-for-inference-using-the-http-api]\n\
  \  - name: InteractiveLogin\n    type: sso\n    mechanism: \"tecton login (browser SSO via configured identity provider)\"\n    audience: Python SDK + CLI (human users)\n    sources: [https://docs.tecton.ai/docs/cli]\naccess_control:\n  model: RBAC\n  principals: [User, Service Account]\n  docs: https://docs.tecton.ai/docs/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecton/refs/heads/main/authentication/tecton-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Machine Learning
- Feature Store
- Feature Platform
- MLOps
- Artificial Intelligence
- Real-Time Data
- SDK
---
