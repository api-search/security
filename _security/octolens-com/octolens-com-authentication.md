---
anonymous_access: false
api_key_in: []
api_specs:
- filename: octolens-com-agency-api-openapi.yml
  format: yaml
  label: Octolens Agency API
  slug: octolens-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-agency-api-openapi.yml
- filename: octolens-com-ai-api-openapi.yml
  format: yaml
  label: Octolens AI API
  slug: octolens-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-ai-api-openapi.yml
- filename: octolens-com-analytics-api-openapi.yml
  format: yaml
  label: Octolens Analytics API
  slug: octolens-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-analytics-api-openapi.yml
- filename: octolens-com-attention-api-openapi.yml
  format: yaml
  label: Octolens Attention API
  slug: octolens-com-attention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-attention-api-openapi.yml
- filename: octolens-com-auth-api-openapi.yml
  format: yaml
  label: Octolens Auth API
  slug: octolens-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-auth-api-openapi.yml
- filename: octolens-com-feedback-api-openapi.yml
  format: yaml
  label: Octolens Feedback API
  slug: octolens-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-feedback-api-openapi.yml
- filename: octolens-com-feeds-api-openapi.yml
  format: yaml
  label: Octolens Feeds API
  slug: octolens-com-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-feeds-api-openapi.yml
- filename: octolens-com-filters-api-openapi.yml
  format: yaml
  label: Octolens Filters API
  slug: octolens-com-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-filters-api-openapi.yml
- filename: octolens-com-integrations-api-openapi.yml
  format: yaml
  label: Octolens Integrations API
  slug: octolens-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-integrations-api-openapi.yml
- filename: octolens-com-keywords-api-openapi.yml
  format: yaml
  label: Octolens Keywords API
  slug: octolens-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-keywords-api-openapi.yml
- filename: octolens-com-members-api-openapi.yml
  format: yaml
  label: Octolens Members API
  slug: octolens-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-members-api-openapi.yml
- filename: octolens-com-mentions-api-openapi.yml
  format: yaml
  label: Octolens Mentions API
  slug: octolens-com-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-mentions-api-openapi.yml
- filename: octolens-com-notifications-api-openapi.yml
  format: yaml
  label: Octolens Notifications API
  slug: octolens-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-notifications-api-openapi.yml
- filename: octolens-com-onboarding-api-openapi.yml
  format: yaml
  label: Octolens Onboarding API
  slug: octolens-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-onboarding-api-openapi.yml
- filename: octolens-com-organization-api-openapi.yml
  format: yaml
  label: Octolens Organization API
  slug: octolens-com-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-organization-api-openapi.yml
- filename: octolens-com-search-api-openapi.yml
  format: yaml
  label: Octolens Search API
  slug: octolens-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-search-api-openapi.yml
- filename: octolens-com-setup-api-openapi.yml
  format: yaml
  label: Octolens Setup API
  slug: octolens-com-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octolens-com/openapi/octolens-com-setup-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Octolens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octolens declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Octolens
provider_slug: octolens-com
scheme_count: 1
schemes:
- evidence: 'Authorization string header required Clerk API key. Create one in Settings → API Keys. Pass as Authorization: Bearer <key> .'
  header: Authorization
  how_to_obtain: Create a Clerk API key in Settings → API Keys.
  location: header
  name: Bearer
  type: http-bearer
slug: octolens-com-authentication
source_filename: octolens-com-authentication.yml
source_heading: Authentication Profile
source_url: https://octolens.com/docs/api-reference/auth/introspect-the-credential
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://octolens.com/docs/api-reference/auth/introspect-the-credential\nsources:\n- https://octolens.com/docs/api-reference/auth/introspect-the-credential\n- https://octolens.com/docs/cli/contract/auth-preflight\n- https://octolens.com/docs/cli/commands/auth\n- https://octolens.com/docs/cli/concepts/auth-profiles\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization string header required Clerk API key. Create one in Settings → API Keys. Pass as Authorization: Bearer <key> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Clerk API key in Settings → API Keys.\ndocs: https://octolens.com/docs/api-reference/auth/introspect-the-credential\n"
source_yaml_url: https://artifacts.apis.io/octolens-com/authentication/octolens-com-authentication.yml
summary_line: 1 scheme
tags:
- Social Listening
- Artificial Intelligence
- Marketing
- Analytics
---
