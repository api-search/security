---
anonymous_access: false
api_key_in: []
api_specs:
- filename: signatureapi-com-deliverables-api-openapi.yml
  format: yaml
  label: signatureapi-com Deliverables API
  slug: signatureapi-com-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-deliverables-api-openapi.yml
- filename: signatureapi-com-envelopes-api-openapi.yml
  format: yaml
  label: signatureapi-com Envelopes API
  slug: signatureapi-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-envelopes-api-openapi.yml
- filename: signatureapi-com-events-api-openapi.yml
  format: yaml
  label: signatureapi-com Events API
  slug: signatureapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-events-api-openapi.yml
- filename: signatureapi-com-recipients-api-openapi.yml
  format: yaml
  label: signatureapi-com Recipients API
  slug: signatureapi-com-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-recipients-api-openapi.yml
- filename: signatureapi-com-senders-api-openapi.yml
  format: yaml
  label: signatureapi-com Senders API
  slug: signatureapi-com-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-senders-api-openapi.yml
- filename: signatureapi-com-uploads-api-openapi.yml
  format: yaml
  label: signatureapi-com Uploads API
  slug: signatureapi-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-uploads-api-openapi.yml
- filename: signatureapi-com-webhooks-api-openapi.yml
  format: yaml
  label: signatureapi-com Webhooks API
  slug: signatureapi-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-webhooks-api-openapi.yml
auth_types: []
description: SignatureAPI uses API key authentication to secure access to your account and ensure only authorized requests can create, modify, or access your envelopes and documents.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Signatureapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: signatureapi-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: signatureapi-com
provider_slug: signatureapi-com
scheme_count: 1
schemes:
- evidence: All API requests require authentication using an API key passed in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Navigate to the SignatureAPI Dashboard and copy your test API key from the API Keys section.
  location: header
  name: X-API-Key
  type: apiKey
slug: signatureapi-com-authentication
source_filename: signatureapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://signatureapi.com/docs/api/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://signatureapi.com/docs/api/authentication\nsources:\n- https://signatureapi.com/docs/api/authentication\n- https://signatureapi.com/docs/api/resources/ceremonies/authentication/overview\n- https://signatureapi.com/docs/api/resources/ceremonies/authentication/email-link\n- https://signatureapi.com/docs/api/resources/ceremonies/authentication/email-code\ndescription: SignatureAPI uses API key authentication to secure access to your account and ensure only authorized requests can create, modify,\n  or access your envelopes and documents.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: All API requests require authentication using an API key passed in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Navigate to the SignatureAPI Dashboard and copy your test API key from the API Keys section.\nnote: Recipient authentication methods (email_link,\
  \ email_code, custom) are for signing ceremonies and not for client API authentication.\ndocs: https://signatureapi.com/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/signatureapi-com/authentication/signatureapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- ElectronicSignature
- API
- SaaS
- Compliance
- Automation
---
