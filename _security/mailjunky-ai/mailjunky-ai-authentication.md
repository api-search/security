---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailjunky-ai-analytics-api-openapi.yml
  format: yaml
  label: mailjunky-ai Analytics API
  slug: mailjunky-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-analytics-api-openapi.yml
- filename: mailjunky-ai-auth-api-openapi.yml
  format: yaml
  label: mailjunky-ai Auth API
  slug: mailjunky-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-auth-api-openapi.yml
- filename: mailjunky-ai-contacts-api-openapi.yml
  format: yaml
  label: mailjunky-ai Contacts API
  slug: mailjunky-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-contacts-api-openapi.yml
- filename: mailjunky-ai-emails-api-openapi.yml
  format: yaml
  label: mailjunky-ai Emails API
  slug: mailjunky-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-emails-api-openapi.yml
- filename: mailjunky-ai-events-api-openapi.yml
  format: yaml
  label: mailjunky-ai Events API
  slug: mailjunky-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-events-api-openapi.yml
- filename: mailjunky-ai-health-api-openapi.yml
  format: yaml
  label: mailjunky-ai Health API
  slug: mailjunky-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailjunky-ai/openapi/mailjunky-ai-health-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailjunky Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: mailjunky-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mailjunky-ai
provider_slug: mailjunky-ai
scheme_count: 1
schemes:
- evidence: Logto's MailJunky connector calls MailJunky's email API ( POST /api/v1/emails/send ) with your API key as a Bearer token.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: mailjunky-ai-authentication
source_filename: mailjunky-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mailjunky.ai/blog/send-logto-auth-emails-with-mailjunky
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailjunky.ai/blog/send-logto-auth-emails-with-mailjunky\nsources:\n- https://mailjunky.ai/blog/send-logto-auth-emails-with-mailjunky\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Logto's MailJunky connector calls MailJunky's email API ( POST /api/v1/emails/send ) with your API key as a Bearer token.\n  location: header\n  header: Authorization\ndocs: https://mailjunky.ai/blog/send-logto-auth-emails-with-mailjunky\n"
source_yaml_url: https://artifacts.apis.io/mailjunky-ai/authentication/mailjunky-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email Marketing
- AI
- Automation
- Analytics
---
