---
anonymous_access: false
api_key_in: []
api_specs:
- filename: influship-com-creator-emails-api-openapi.yml
  format: yaml
  label: Influship Creator Emails API
  slug: influship-com-creator-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-creator-emails-api-openapi.yml
- filename: influship-com-creators-api-openapi.yml
  format: yaml
  label: Influship Creators API
  slug: influship-com-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-creators-api-openapi.yml
- filename: influship-com-live-scraping-api-openapi.yml
  format: yaml
  label: Influship Live Scraping API
  slug: influship-com-live-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-live-scraping-api-openapi.yml
- filename: influship-com-posts-api-openapi.yml
  format: yaml
  label: Influship Posts API
  slug: influship-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-posts-api-openapi.yml
- filename: influship-com-profiles-api-openapi.yml
  format: yaml
  label: Influship Profiles API
  slug: influship-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-profiles-api-openapi.yml
- filename: influship-com-ready-api-openapi.yml
  format: yaml
  label: Influship Ready API
  slug: influship-com-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-ready-api-openapi.yml
- filename: influship-com-search-api-openapi.yml
  format: yaml
  label: Influship Search API
  slug: influship-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-search-api-openapi.yml
- filename: influship-com-shortlists-api-openapi.yml
  format: yaml
  label: Influship Shortlists API
  slug: influship-com-shortlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influship-com/openapi/influship-com-shortlists-api-openapi.yml
auth_types: []
description: Authentication methods for Influship API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Influship Authentication
name_suffix: Authentication
oauth_flows: []
overview: Influship declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Influship
provider_slug: influship-com
scheme_count: 2
schemes:
- evidence: Use an API key for direct server-side requests, OAuth for linked accounts, or a supported payment protocol for keyless requests.
  header: X-API-Key
  how_to_obtain: Create a key in the developer dashboard (https://developers.influship.com).
  location: header
  name: API key
  type: apiKey
- evidence: 'OAuth | `Authorization: Bearer <access_token>` | Complete account linking in your client; see MCP setup.'
  header: Authorization
  how_to_obtain: Complete account linking in your client; see MCP setup (https://docs.influship.com/guides/mcp-server.md).
  location: header
  name: OAuth
  type: oauth2
slug: influship-com-authentication
source_filename: influship-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.influship.com/guides/authentication.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.influship.com/guides/authentication.md\nsources:\n- https://docs.influship.com/guides/authentication.md\n- https://developers.influship.com/auth/signup\n- https://docs.influship.com/quickstart.md\n- https://docs.influship.com/sdks/index.md\ndescription: Authentication methods for Influship API\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Use an API key for direct server-side requests, OAuth for linked accounts, or a supported payment protocol for keyless requests.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the developer dashboard (https://developers.influship.com).\n- type: oauth2\n  name: OAuth\n  evidence: 'OAuth | `Authorization: Bearer <access_token>` | Complete account linking in your client; see MCP setup.'\n  location: header\n  header: Authorization\n  how_to_obtain: Complete account linking in your client; see MCP\
  \ setup (https://docs.influship.com/guides/mcp-server.md).\ndocs: https://docs.influship.com/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/influship-com/authentication/influship-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Influencer Marketing
- Creator Search
- Data Analytics
- Marketing
---
