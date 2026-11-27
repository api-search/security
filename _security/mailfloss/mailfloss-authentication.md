---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailfloss-account-api-openapi.yml
  format: yaml
  label: mailfloss Account API
  slug: mailfloss-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-account-api-openapi.yml
- filename: mailfloss-batch-api-openapi.yml
  format: yaml
  label: mailfloss Batch API
  slug: mailfloss-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-batch-api-openapi.yml
- filename: mailfloss-integrations-api-openapi.yml
  format: yaml
  label: mailfloss Integrations API
  slug: mailfloss-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-integrations-api-openapi.yml
- filename: mailfloss-privacy-api-openapi.yml
  format: yaml
  label: mailfloss Privacy API
  slug: mailfloss-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-privacy-api-openapi.yml
- filename: mailfloss-reports-api-openapi.yml
  format: yaml
  label: mailfloss Reports API
  slug: mailfloss-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-reports-api-openapi.yml
- filename: mailfloss-team-api-openapi.yml
  format: yaml
  label: mailfloss Team API
  slug: mailfloss-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-team-api-openapi.yml
- filename: mailfloss-verification-api-openapi.yml
  format: yaml
  label: mailfloss Verification API
  slug: mailfloss-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-verification-api-openapi.yml
- filename: mailfloss-verification-api-openapi.yml
  format: yaml
  label: mailfloss API
  slug: mailfloss-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-verification-api-openapi.yml
- filename: mailfloss-webhooks-api-openapi.yml
  format: yaml
  label: mailfloss Webhooks API
  slug: mailfloss-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-webhooks-api-openapi.yml
- filename: mailfloss-batch-verify-api-openapi.yml
  format: yaml
  label: Mailfloss batch verify API
  slug: mailfloss-batch-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-batch-verify-api-openapi.yml
- filename: mailfloss-verify-api-openapi.yml
  format: yaml
  label: Mailfloss Verify API
  slug: mailfloss-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-verify-api-openapi.yml
auth_types: []
description: Mailfloss API authentication methods
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mailfloss Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailfloss declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mailfloss
provider_slug: mailfloss
scheme_count: 2
schemes:
- evidence: 'Send your key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Create an API key in the mailfloss dashboard under Developers → API keys.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: All of your requests needs to be authenticated with your API key and passed in as a query parameter `api_key`.
  how_to_obtain: Create an API key in the mailfloss dashboard under Developers → API keys.
  location: query
  name: Legacy api_key query parameter
  type: apiKey
slug: mailfloss-authentication
source_filename: mailfloss-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.mailfloss.com/email-verification-authentication.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.mailfloss.com/email-verification-authentication.md\nsources:\n- https://developers.mailfloss.com/email-verification-authentication.md\n- https://developers.mailfloss.com/authentication.md\n- https://developers.mailfloss.com/authentication\n- https://docs.mailfloss.com/how-to-enable-two-factor-authentication-2fa\ndescription: Mailfloss API authentication methods\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send your key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the mailfloss dashboard under Developers → API keys.\n- type: apiKey\n  name: Legacy api_key query parameter\n  evidence: All of your requests needs to be authenticated with your API key and passed in as a query parameter `api_key`.\n  location: query\n  how_to_obtain: Create an API key in the mailfloss dashboard\
  \ under Developers → API keys.\nnote: No OAuth2 flows are documented for Mailfloss; only API key based schemes are provided.\ndocs: https://developers.mailfloss.com/email-verification-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/mailfloss/authentication/mailfloss-authentication.yml
summary_line: 2 schemes
tags:
- Email Verification
- Marketing
- Software-as-a-Service
- Automation
- Deliverability
---
