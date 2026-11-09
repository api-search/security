---
anonymous_access: false
api_key_in: []
api_specs:
- filename: citeladder-com-actions-api-openapi.yml
  format: yaml
  label: CiteLadder Actions API
  slug: citeladder-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-actions-api-openapi.yml
- filename: citeladder-com-ai-traffic-api-openapi.yml
  format: yaml
  label: CiteLadder AI Traffic API
  slug: citeladder-com-ai-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-ai-traffic-api-openapi.yml
- filename: citeladder-com-audit-schedules-api-openapi.yml
  format: yaml
  label: CiteLadder Audit Schedules API
  slug: citeladder-com-audit-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-audit-schedules-api-openapi.yml
- filename: citeladder-com-audits-api-openapi.yml
  format: yaml
  label: CiteLadder Audits API
  slug: citeladder-com-audits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-audits-api-openapi.yml
- filename: citeladder-com-business-map-api-openapi.yml
  format: yaml
  label: CiteLadder Business Map API
  slug: citeladder-com-business-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-business-map-api-openapi.yml
- filename: citeladder-com-competitor-suggestions-api-openapi.yml
  format: yaml
  label: CiteLadder Competitor Suggestions API
  slug: citeladder-com-competitor-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-competitor-suggestions-api-openapi.yml
- filename: citeladder-com-competitors-api-openapi.yml
  format: yaml
  label: CiteLadder Competitors API
  slug: citeladder-com-competitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-competitors-api-openapi.yml
- filename: citeladder-com-markets-api-openapi.yml
  format: yaml
  label: CiteLadder Markets API
  slug: citeladder-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-markets-api-openapi.yml
- filename: citeladder-com-performance-api-openapi.yml
  format: yaml
  label: CiteLadder Performance API
  slug: citeladder-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-performance-api-openapi.yml
- filename: citeladder-com-projects-api-openapi.yml
  format: yaml
  label: CiteLadder Projects API
  slug: citeladder-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-projects-api-openapi.yml
- filename: citeladder-com-prompt-sets-api-openapi.yml
  format: yaml
  label: CiteLadder Prompt Sets API
  slug: citeladder-com-prompt-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-prompt-sets-api-openapi.yml
- filename: citeladder-com-prompts-api-openapi.yml
  format: yaml
  label: CiteLadder Prompts API
  slug: citeladder-com-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-prompts-api-openapi.yml
- filename: citeladder-com-search-intelligence-api-openapi.yml
  format: yaml
  label: CiteLadder Search Intelligence API
  slug: citeladder-com-search-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-search-intelligence-api-openapi.yml
- filename: citeladder-com-site-crawls-api-openapi.yml
  format: yaml
  label: CiteLadder Site Crawls API
  slug: citeladder-com-site-crawls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-site-crawls-api-openapi.yml
- filename: citeladder-com-site-health-api-openapi.yml
  format: yaml
  label: CiteLadder Site Health API
  slug: citeladder-com-site-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-site-health-api-openapi.yml
- filename: citeladder-com-topics-api-openapi.yml
  format: yaml
  label: CiteLadder Topics API
  slug: citeladder-com-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-topics-api-openapi.yml
- filename: citeladder-com-visibility-api-openapi.yml
  format: yaml
  label: CiteLadder Visibility API
  slug: citeladder-com-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citeladder-com/openapi/citeladder-com-visibility-api-openapi.yml
auth_types: []
description: CiteLadder authentication uses browser sign‑in (OAuth) with the read scope citeladder:read, plus citeladder:write when allowed.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Citeladder Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CiteLadder declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CiteLadder
provider_slug: citeladder-com
scheme_count: 1
schemes:
- evidence: The connection uses browser sign-in (OAuth) with the read scope citeladder:read , plus citeladder:write when you tick Allow changes on the consent page.
  flows:
  - authorization_code
  how_to_obtain: Sign in to CiteLadder via the browser consent page; the client redirects to CiteLadder’s OAuth consent screen where the user authorizes the requested scopes.
  name: OAuth
  scopes:
  - citeladder:read
  - citeladder:write
  type: oauth2
slug: citeladder-com-authentication
source_filename: citeladder-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.citeladder.com/quickstart/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.citeladder.com/quickstart/\nsources:\n- https://docs.citeladder.com/quickstart/\n- https://docs.citeladder.com/mcp/connect/\ndescription: CiteLadder authentication uses browser sign‑in (OAuth) with the read scope citeladder:read, plus citeladder:write when allowed.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: The connection uses browser sign-in (OAuth) with the read scope citeladder:read , plus citeladder:write when you tick Allow changes\n    on the consent page.\n  flows:\n  - authorization_code\n  scopes:\n  - citeladder:read\n  - citeladder:write\n  how_to_obtain: Sign in to CiteLadder via the browser consent page; the client redirects to CiteLadder’s OAuth consent screen where the user\n    authorizes the requested scopes.\ndocs: https://docs.citeladder.com/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/citeladder-com/authentication/citeladder-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Visibility
- Search
- Citations
- Analytics
---
