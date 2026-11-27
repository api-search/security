---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gemini Notebook (NotebookLM) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemini Notebook (NotebookLM) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gemini Notebook (NotebookLM)
provider_slug: notebooklm
scheme_count: 1
schemes:
- description: Google Cloud OAuth 2.0 user access token sent as "Authorization:Bearer $(gcloud auth print-access-token)" after "gcloud auth login". The user needs a Gemini Notebook Enterprise license and the Cloud NotebookLM User role (roles/discoveryengine.notebookLmUser).
  scheme: bearer
  type: oauth2
slug: notebooklm-authentication
source_filename: notebooklm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Gemini Notebook Enterprise API authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://docs.cloud.google.com/gemini/enterprise/notebooklm-enterprise/docs/api-notebooks\ndocs: https://docs.cloud.google.com/gemini/enterprise/notebooklm-enterprise/docs/api-notebooks\nschemes:\n- type: oauth2\n  scheme: bearer\n  description: 'Google Cloud OAuth 2.0 user access token sent as \"Authorization:Bearer $(gcloud auth print-access-token)\" after \"gcloud auth login\". The user needs a Gemini Notebook Enterprise license and the Cloud NotebookLM User role (roles/discoveryengine.notebookLmUser).'\n"
source_yaml_url: https://artifacts.apis.io/notebooklm/authentication/notebooklm-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Research
- Knowledge Management
- Document Analysis
- Generative AI
- Google
- Notebooks
---
