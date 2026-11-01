---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finchnode-com-api-openapi.yml
  format: yaml
  label: FinchNode Developer API API
  slug: finchnode-developer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finchnode-com/openapi/_original/finchnode-com-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finchnode Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: finchnode-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: finchnode-com
provider_slug: finchnode-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer $FINCHNODE_API_KEY'
  header: Authorization
  location: header
  name: FinchNode API Key
  type: http-bearer
- evidence: A SMART standalone launch is an OAuth 2.0 authorization-code flow with FHIR-specific discovery, audience, scopes, and patient context.
  flows:
  - authorization_code
  name: SMART on FHIR
  scopes:
  - openid
  - fhirUser
  - launch/patient
  - patient/*.rs
  type: oauth2
slug: finchnode-com-authentication
source_filename: finchnode-com-authentication.yml
source_heading: Authentication Profile
source_url: https://finchnode.com/blog/smart-on-fhir-oauth-pkce-react-node.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finchnode.com/blog/smart-on-fhir-oauth-pkce-react-node.md\nsources:\n- https://finchnode.com/blog/smart-on-fhir-oauth-pkce-react-node.md\n- https://finchnode.com/docs/ai-agents/agent-credentials.md\n- https://finchnode.com/docs/ai-agents/agent-credentials\n- https://finchnode.com/docs/get-started/quickstart.md\nschemes:\n- type: http-bearer\n  name: FinchNode API Key\n  evidence: 'Authorization: Bearer $FINCHNODE_API_KEY'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: SMART on FHIR\n  evidence: A SMART standalone launch is an OAuth 2.0 authorization-code flow with FHIR-specific discovery, audience, scopes, and patient context.\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - fhirUser\n  - launch/patient\n  - patient/*.rs\ndocs: https://finchnode.com/blog/smart-on-fhir-oauth-pkce-react-node.md\n"
source_yaml_url: https://artifacts.apis.io/finchnode-com/authentication/finchnode-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- API
- EHR
- OpenData
---
