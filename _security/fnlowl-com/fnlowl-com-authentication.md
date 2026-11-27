---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fnlowl-com-advisor-api-openapi.yml
  format: yaml
  label: FnlOwl Advisor API
  slug: fnlowl-com-advisor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-advisor-api-openapi.yml
- filename: fnlowl-com-analytics-api-openapi.yml
  format: yaml
  label: FnlOwl Analytics API
  slug: fnlowl-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-analytics-api-openapi.yml
- filename: fnlowl-com-billing-api-openapi.yml
  format: yaml
  label: FnlOwl Billing API
  slug: fnlowl-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-billing-api-openapi.yml
- filename: fnlowl-com-campaigns-api-openapi.yml
  format: yaml
  label: FnlOwl Campaigns API
  slug: fnlowl-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-campaigns-api-openapi.yml
- filename: fnlowl-com-capture-api-openapi.yml
  format: yaml
  label: FnlOwl Capture API
  slug: fnlowl-com-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-capture-api-openapi.yml
- filename: fnlowl-com-chat-api-openapi.yml
  format: yaml
  label: FnlOwl Chat API
  slug: fnlowl-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-chat-api-openapi.yml
- filename: fnlowl-com-developer-api-openapi.yml
  format: yaml
  label: FnlOwl Developer API
  slug: fnlowl-com-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-developer-api-openapi.yml
- filename: fnlowl-com-email-api-openapi.yml
  format: yaml
  label: FnlOwl Email API
  slug: fnlowl-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-email-api-openapi.yml
- filename: fnlowl-com-identity-api-openapi.yml
  format: yaml
  label: FnlOwl Identity API
  slug: fnlowl-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-identity-api-openapi.yml
- filename: fnlowl-com-integrations-api-openapi.yml
  format: yaml
  label: FnlOwl Integrations API
  slug: fnlowl-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-integrations-api-openapi.yml
- filename: fnlowl-com-leads-api-openapi.yml
  format: yaml
  label: FnlOwl Leads API
  slug: fnlowl-com-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-leads-api-openapi.yml
- filename: fnlowl-com-oauth-api-openapi.yml
  format: yaml
  label: FnlOwl OAuth API
  slug: fnlowl-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-oauth-api-openapi.yml
- filename: fnlowl-com-sequences-api-openapi.yml
  format: yaml
  label: FnlOwl Sequences API
  slug: fnlowl-com-sequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-sequences-api-openapi.yml
- filename: fnlowl-com-settings-api-openapi.yml
  format: yaml
  label: FnlOwl Settings API
  slug: fnlowl-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-settings-api-openapi.yml
- filename: fnlowl-com-signin-api-openapi.yml
  format: yaml
  label: FnlOwl Signin API
  slug: fnlowl-com-signin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-signin-api-openapi.yml
- filename: fnlowl-com-transactional-api-openapi.yml
  format: yaml
  label: FnlOwl Transactional API
  slug: fnlowl-com-transactional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-transactional-api-openapi.yml
- filename: fnlowl-com-widgets-api-openapi.yml
  format: yaml
  label: FnlOwl Widgets API
  slug: fnlowl-com-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fnlowl-com/openapi/fnlowl-com-widgets-api-openapi.yml
auth_types: []
description: Authentication schemes for FnlOwl API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FnlOwl Authentication
name_suffix: Authentication
oauth_flows: []
overview: FnlOwl declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FnlOwl
provider_slug: fnlowl-com
scheme_count: 1
schemes:
- evidence: 'Send it Authorization: Bearer fnlk_...'
  header: Authorization
  how_to_obtain: Create a key in Settings → API, give it a name, choose its scopes, and copy the shown key.
  location: header
  name: Bearer
  scopes:
  - read
  - write
  - publish
  type: http-bearer
slug: fnlowl-com-authentication
source_filename: fnlowl-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fnlowl.com/docs/api/authentication/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fnlowl.com/docs/api/authentication/\nsources:\n- https://fnlowl.com/docs/api/authentication/\n- https://fnlowl.com/docs/get-started/quickstart/\n- https://fnlowl.com/docs/api/\ndescription: Authentication schemes for FnlOwl API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it Authorization: Bearer fnlk_...'\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - write\n  - publish\n  how_to_obtain: Create a key in Settings → API, give it a name, choose its scopes, and copy the shown key.\nnote: No OAuth flows or other authentication methods are documented on the provided pages.\ndocs: https://fnlowl.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/fnlowl-com/authentication/fnlowl-com-authentication.yml
summary_line: 1 scheme
tags:
- Lead Capture
- Email Automation
- Software-as-a-Service
- Marketing Tools
- Small Business
---
