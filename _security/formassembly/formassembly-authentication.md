---
api_key_in: []
api_specs:
- filename: formassembly-aggregates-api-openapi.yml
  format: yaml
  label: FormAssembly Aggregates API
  slug: formassembly-aggregates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-aggregates-api-openapi.yml
- filename: formassembly-connectors-api-openapi.yml
  format: yaml
  label: FormAssembly Connectors API
  slug: formassembly-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-connectors-api-openapi.yml
- filename: formassembly-form-elements-api-openapi.yml
  format: yaml
  label: FormAssembly Form Elements API
  slug: formassembly-form-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-form-elements-api-openapi.yml
- filename: formassembly-forms-api-openapi.yml
  format: yaml
  label: FormAssembly Forms API
  slug: formassembly-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-forms-api-openapi.yml
- filename: formassembly-oauth2-api-openapi.yml
  format: yaml
  label: FormAssembly OAuth2 API
  slug: formassembly-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-oauth2-api-openapi.yml
- filename: formassembly-responses-api-openapi.yml
  format: yaml
  label: FormAssembly Responses API
  slug: formassembly-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-responses-api-openapi.yml
- filename: formassembly-themes-api-openapi.yml
  format: yaml
  label: FormAssembly Themes API
  slug: formassembly-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-themes-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Formassembly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FormAssembly secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FormAssembly
provider_slug: formassembly
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://app.formassembly.com/oauth/login
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://app.formassembly.com/oauth/access_token
  name: oauth2
  sources:
  - openapi/formassembly-formassembly-api-openapi.yml
  type: oauth2
slug: formassembly-authentication
source_filename: formassembly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formassembly-formassembly-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.formassembly.com/oauth/login\n    tokenUrl: https://app.formassembly.com/oauth/access_token\n    scopes: 0\n  sources:\n  - openapi/formassembly-formassembly-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/authentication/formassembly-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Forms
- Data Collection
- Salesforce
- Enterprise
- HIPAA
- Compliance
- Government
- FedRAMP
- Workflows
- E-Signatures
---
