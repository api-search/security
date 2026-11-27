---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumierepaycheck-org-monitoring-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Monitoring API
  slug: lumierepaycheck-org-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-monitoring-api-openapi.yml
- filename: lumierepaycheck-org-security-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Security API
  slug: lumierepaycheck-org-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-security-api-openapi.yml
- filename: lumierepaycheck-org-trust-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Trust API
  slug: lumierepaycheck-org-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-trust-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lumière PayCheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumière PayCheck declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lumière PayCheck
provider_slug: lumierepaycheck-org
scheme_count: 2
schemes:
- evidence: 'Copy curl https://lumierepaycheck.org/v1/authorize \ -H "Authorization: Bearer $PAYCHECK_AGENT_KEY" -H "content-type: application/json" \'
  header: Authorization
  how_to_obtain: Free API key is emailed to you after requesting it on the Free API key page.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'It asks for a credential for that seller and sends it as the X-PayCheck-Agent header: Copy curl -X POST https://lumierepaycheck.org/v1/agents/credential -H "Authorization: Bearer $PAYCHECK_AGENT_KEY" \ -H "content-type: application/json" -d ''{"audience":"api.seller.example"}'''
  header: X-PayCheck-Agent
  how_to_obtain: Agent obtains a credential by POST /v1/agents/credential using its agent key.
  location: header
  name: Agent credential
  type: apiKey
slug: lumierepaycheck-org-authentication
source_filename: lumierepaycheck-org-authentication.yml
source_heading: Authentication Profile
source_url: https://lumierepaycheck.org/free-key
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lumierepaycheck.org/free-key\nsources:\n- https://lumierepaycheck.org/free-key\n- https://lumierepaycheck.org/docs/integration\n- https://lumierepaycheck.org/setup\n- https://lumierepaycheck.org/docs/quickstart\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Copy curl https://lumierepaycheck.org/v1/authorize \\ -H \"Authorization: Bearer $PAYCHECK_AGENT_KEY\" -H \"content-type: application/json\"\n    \\'\n  location: header\n  header: Authorization\n  how_to_obtain: Free API key is emailed to you after requesting it on the Free API key page.\n- type: apiKey\n  name: Agent credential\n  evidence: 'It asks for a credential for that seller and sends it as the X-PayCheck-Agent header: Copy curl -X POST https://lumierepaycheck.org/v1/agents/credential\n    -H \"Authorization: Bearer $PAYCHECK_AGENT_KEY\" \\ -H \"content-type: application/json\" -d ''{\"audience\"\
  :\"api.seller.example\"}'''\n  location: header\n  header: X-PayCheck-Agent\n  how_to_obtain: Agent obtains a credential by POST /v1/agents/credential using its agent key.\ndocs: https://lumierepaycheck.org/free-key\n"
source_yaml_url: https://artifacts.apis.io/lumierepaycheck-org/authentication/lumierepaycheck-org-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Payments
- Automation
- Agents
---
