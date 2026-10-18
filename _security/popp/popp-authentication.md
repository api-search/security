---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: popp-agents-api-openapi.yml
  format: yaml
  label: Popp Agents API
  slug: popp-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-agents-api-openapi.yml
- filename: popp-analysis-api-openapi.yml
  format: yaml
  label: Popp Analysis API
  slug: popp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-analysis-api-openapi.yml
- filename: popp-ats-api-openapi.yml
  format: yaml
  label: Popp ATS API
  slug: popp-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-ats-api-openapi.yml
- filename: popp-campaigns-api-openapi.yml
  format: yaml
  label: Popp Campaigns API
  slug: popp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-campaigns-api-openapi.yml
- filename: popp-candidate-lists-api-openapi.yml
  format: yaml
  label: Popp Candidate Lists API
  slug: popp-candidate-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidate-lists-api-openapi.yml
- filename: popp-candidates-api-openapi.yml
  format: yaml
  label: Popp Candidates API
  slug: popp-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidates-api-openapi.yml
- filename: popp-conversations-api-openapi.yml
  format: yaml
  label: Popp Conversations API
  slug: popp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-conversations-api-openapi.yml
- filename: popp-custom-fields-beta-api-openapi.yml
  format: yaml
  label: Popp Custom Fields (Beta) API
  slug: popp-custom-fields-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-custom-fields-beta-api-openapi.yml
- filename: popp-document-credentials-api-openapi.yml
  format: yaml
  label: Popp Document Credentials API
  slug: popp-document-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-document-credentials-api-openapi.yml
- filename: popp-documents-api-openapi.yml
  format: yaml
  label: Popp Documents API
  slug: popp-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-documents-api-openapi.yml
- filename: popp-organization-configuration-api-openapi.yml
  format: yaml
  label: Popp Organization Configuration API
  slug: popp-organization-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organization-configuration-api-openapi.yml
- filename: popp-organizations-api-openapi.yml
  format: yaml
  label: Popp Organizations API
  slug: popp-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organizations-api-openapi.yml
- filename: popp-scheduling-api-openapi.yml
  format: yaml
  label: Popp Scheduling API
  slug: popp-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-scheduling-api-openapi.yml
- filename: popp-tags-api-openapi.yml
  format: yaml
  label: Popp Tags API
  slug: popp-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-tags-api-openapi.yml
- filename: popp-templates-api-openapi.yml
  format: yaml
  label: Popp Templates API
  slug: popp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-templates-api-openapi.yml
- filename: popp-users-api-openapi.yml
  format: yaml
  label: Popp Users API
  slug: popp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-users-api-openapi.yml
- filename: popp-webhooks-api-openapi.yml
  format: yaml
  label: Popp Webhooks API
  slug: popp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-webhooks-api-openapi.yml
- filename: popp-workflows-api-openapi.yml
  format: yaml
  label: Popp Workflows API
  slug: popp-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Popp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Popp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Popp
provider_slug: popp
scheme_count: 2
schemes:
- description: Secret key authenticating the request; grants full access to the organization's data.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - https://docs.joinpopp.com/docs/authentication-guide
  type: apiKey
- description: Unique identifier for the caller's subaccount (organization) in Popp; required alongside the API key.
  in: header
  name: OrganizationId
  parameter: x-organization-id
  sources:
  - https://docs.joinpopp.com/docs/authentication-guide
  type: apiKey
slug: popp-authentication
source_filename: popp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.joinpopp.com/docs/authentication-guide\ndocs: https://docs.joinpopp.com/docs/authentication-guide\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    Every request requires TWO headers: a secret API key and the caller's\n    Organization ID. No OAuth or OpenID Connect surface is documented.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: Secret key authenticating the request; grants full access to the organization's data.\n    sources: [https://docs.joinpopp.com/docs/authentication-guide]\n  - name: OrganizationId\n    type: apiKey\n    in: header\n    parameter: x-organization-id\n    description: Unique identifier for the caller's subaccount (organization) in Popp; required alongside the API key.\n    sources: [https://docs.joinpopp.com/docs/authentication-guide]\ncredentials_portal: https://app.joinpopp.com/developer/keys\n\
  key_management:\n  self_serve: true\n  features: [create, expiry, revocation]\n  docs: https://docs.joinpopp.com/docs/api-key-management\nexample_request: |\n  curl -X GET \"https://api.joinpopp.com/v1/conversations\" \\\n    -H \"x-api-key: YOUR_API_KEY\" \\\n    -H \"x-organization-id: YOUR_ORGANIZATION_ID\" \\\n    -H \"Content-Type: application/json\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/authentication/popp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Recruiting
- Staffing
- Hiring
- Conversational AI
- Automation
- Scheduling
- Workflows
- Webhook
- MCP
- Agents
---
