---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feedboss-ai-openapi-generated.yml
  format: yaml
  label: FeedBoss API
  slug: feedboss-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedboss-ai/openapi/_ae-authored/feedboss-ai-openapi-generated.yml
auth_types: []
description: FeedBoss API uses a Service API Key sent in a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FeedBoss Authentication
name_suffix: Authentication
oauth_flows: []
overview: FeedBoss declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FeedBoss
provider_slug: feedboss-ai
scheme_count: 1
schemes:
- evidence: Include the API key in the x-api-key header of your HTTP requests.
  header: x-api-key
  how_to_obtain: Navigate to Workspace Settings → Service API Keys, click Create New Key, give it a name, and copy the key.
  location: header
  name: Service API Key
  type: apiKey
slug: feedboss-ai-authentication
source_filename: feedboss-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.feedboss.ai/docs/api/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.feedboss.ai/docs/api/authentication\nsources:\n- https://www.feedboss.ai/docs/api/authentication\n- https://www.feedboss.ai/docs/features/white-label\n- https://www.feedboss.ai/docs/features/white-label\n- https://www.feedboss.ai/docs/getting-started\ndescription: FeedBoss API uses a Service API Key sent in a custom header.\nschemes:\n- type: apiKey\n  name: Service API Key\n  evidence: Include the API key in the x-api-key header of your HTTP requests.\n  location: header\n  header: x-api-key\n  how_to_obtain: Navigate to Workspace Settings → Service API Keys, click Create New Key, give it a name, and copy the key.\nnote: No OAuth2, HTTP basic, bearer, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://www.feedboss.ai/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/feedboss-ai/authentication/feedboss-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Marketing
- Content Automation
- LinkedIn
---
