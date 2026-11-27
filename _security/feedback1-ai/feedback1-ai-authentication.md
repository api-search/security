---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feedback1-ai-accounts-api-openapi.yml
  format: yaml
  label: Feedback1 Accounts API
  slug: feedback1-ai-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-accounts-api-openapi.yml
- filename: feedback1-ai-api-keys-api-openapi.yml
  format: yaml
  label: Feedback1 API Keys API
  slug: feedback1-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-api-keys-api-openapi.yml
- filename: feedback1-ai-banners-public-api-openapi.yml
  format: yaml
  label: Feedback1 Banners Public API
  slug: feedback1-ai-banners-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-banners-public-api-openapi.yml
- filename: feedback1-ai-changelog-api-openapi.yml
  format: yaml
  label: Feedback1 Changelog API
  slug: feedback1-ai-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-changelog-api-openapi.yml
- filename: feedback1-ai-contacts-api-openapi.yml
  format: yaml
  label: Feedback1 Contacts API
  slug: feedback1-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-contacts-api-openapi.yml
- filename: feedback1-ai-deals-api-openapi.yml
  format: yaml
  label: Feedback1 Deals API
  slug: feedback1-ai-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-deals-api-openapi.yml
- filename: feedback1-ai-features-api-openapi.yml
  format: yaml
  label: Feedback1 Features API
  slug: feedback1-ai-features-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-features-api-openapi.yml
- filename: feedback1-ai-feedback-api-openapi.yml
  format: yaml
  label: Feedback1 Feedback API
  slug: feedback1-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-feedback-api-openapi.yml
- filename: feedback1-ai-products-api-openapi.yml
  format: yaml
  label: Feedback1 Products API
  slug: feedback1-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-products-api-openapi.yml
- filename: feedback1-ai-public-forms-api-openapi.yml
  format: yaml
  label: Feedback1 Public Forms API
  slug: feedback1-ai-public-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-public-forms-api-openapi.yml
- filename: feedback1-ai-roadmap-api-openapi.yml
  format: yaml
  label: Feedback1 Roadmap API
  slug: feedback1-ai-roadmap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-roadmap-api-openapi.yml
- filename: feedback1-ai-roadmap-public-api-openapi.yml
  format: yaml
  label: Feedback1 Roadmap Public API
  slug: feedback1-ai-roadmap-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-roadmap-public-api-openapi.yml
- filename: feedback1-ai-userportal-public-api-openapi.yml
  format: yaml
  label: Feedback1 Userportal Public API
  slug: feedback1-ai-userportal-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-userportal-public-api-openapi.yml
- filename: feedback1-ai-webhooks-api-openapi.yml
  format: yaml
  label: Feedback1 Webhooks API
  slug: feedback1-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-webhooks-api-openapi.yml
- filename: feedback1-ai-widgets-public-api-openapi.yml
  format: yaml
  label: Feedback1 Widgets Public API
  slug: feedback1-ai-widgets-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-widgets-public-api-openapi.yml
- filename: feedback1-ai-youtrack-api-openapi.yml
  format: yaml
  label: Feedback1 You Track API
  slug: feedback1-ai-youtrack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedback1-ai/openapi/feedback1-ai-youtrack-api-openapi.yml
auth_types: []
description: Authentication methods for Feedback1
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Feedback1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feedback1 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Feedback1
provider_slug: feedback1-ai
scheme_count: 2
schemes:
- evidence: Cursor and Claude connect with OAuth. The SSE URL https://app.feedback1.ai/api/mcp/sse still works for mcp-remote.
  header: Authorization
  how_to_obtain: Your client discovers OAuth automatically, opens a browser to sign in to Feedback1, and you pick which product to authorize.
  location: header
  name: OAuth
  type: http-bearer
- evidence: 'All requests require a workspace API key in the Authorization header: Authorization: Bearer <api_key>'
  header: Authorization
  how_to_obtain: Create a Feedback1 workspace API key in Settings → API Keys.
  location: header
  name: API Key
  type: apiKey
slug: feedback1-ai-authentication
source_filename: feedback1-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://feedback1.ai/docs/integrations/mcp
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://feedback1.ai/docs/integrations/mcp\nsources:\n- https://feedback1.ai/docs/integrations/mcp\n- https://feedback1.ai/docs/integrations/api\ndescription: Authentication methods for Feedback1\nschemes:\n- type: http-bearer\n  name: OAuth\n  evidence: Cursor and Claude connect with OAuth. The SSE URL https://app.feedback1.ai/api/mcp/sse still works for mcp-remote.\n  location: header\n  header: Authorization\n  how_to_obtain: Your client discovers OAuth automatically, opens a browser to sign in to Feedback1, and you pick which product to authorize.\n- type: apiKey\n  name: API Key\n  evidence: 'All requests require a workspace API key in the Authorization header: Authorization: Bearer <api_key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Feedback1 workspace API key in Settings → API Keys.\ndocs: https://feedback1.ai/docs/integrations/mcp\n"
source_yaml_url: https://artifacts.apis.io/feedback1-ai/authentication/feedback1-ai-authentication.yml
summary_line: 2 schemes
tags:
- Feedback
- Roadmaps
- Artificial Intelligence
- Software-as-a-Service
- Customer Success
---
