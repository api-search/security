---
anonymous_access: false
api_key_in: []
api_specs:
- filename: campaignstack-io-openapi-generated.yml
  format: yaml
  label: CampaignStack API
  slug: campaignstack-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campaignstack-io/openapi/_ae-authored/campaignstack-io-openapi-generated.yml
auth_types: []
description: Authentication methods published by CampaignStack
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Campaignstack Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: CampaignStack declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CampaignStack
provider_slug: campaignstack-io
scheme_count: 3
schemes:
- evidence: 'Pass the key as a Bearer token in the Authorization header, or in an X-Api-Key header when your client reserves Authorization for its own OAuth token (claude.ai connectors do):'
  header: Authorization
  how_to_obtain: Create an API key in Settings > Personal API keys (user key) or Workspace Settings > API Keys (workspace key).
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Equivalent, for clients that cannot set Authorization -H " X-Api-Key: csu_your_api_key_here "'
  header: X-Api-Key
  how_to_obtain: Create an API key in Settings > Personal API keys (user key) or Workspace Settings > API Keys (workspace key).
  location: header
  name: X-Api-Key header
  type: apiKey
- evidence: For internal service communication, CampaignStack supports a separate authentication method using the X-Runner-Secret header with additional context headers ( x-workspace-id , x-user-id ).
  header: X-Runner-Secret
  location: header
  name: X-Runner-Secret header
  type: other
slug: campaignstack-io-authentication
source_filename: campaignstack-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.campaignstack.io/mcp/authentication/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.campaignstack.io/mcp/authentication/\nsources:\n- https://docs.campaignstack.io/mcp/authentication/\n- https://docs.campaignstack.io/getting-started/quick-start/\n- https://docs.campaignstack.io/guides/claude-desktop/\n- https://docs.campaignstack.io/guides/cursor/\ndescription: Authentication methods published by CampaignStack\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Pass the key as a Bearer token in the Authorization header, or in an X-Api-Key header when your client reserves Authorization for\n    its own OAuth token (claude.ai connectors do):'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings > Personal API keys (user key) or Workspace Settings > API Keys (workspace key).\n- type: apiKey\n  name: X-Api-Key header\n  evidence: 'Equivalent, for clients that cannot set Authorization -H \" X-Api-Key:\
  \ csu_your_api_key_here \"'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create an API key in Settings > Personal API keys (user key) or Workspace Settings > API Keys (workspace key).\n- type: other\n  name: X-Runner-Secret header\n  evidence: For internal service communication, CampaignStack supports a separate authentication method using the X-Runner-Secret header with\n    additional context headers ( x-workspace-id , x-user-id ).\n  location: header\n  header: X-Runner-Secret\ndocs: https://docs.campaignstack.io/mcp/authentication/\n"
source_yaml_url: https://artifacts.apis.io/campaignstack-io/authentication/campaignstack-io-authentication.yml
summary_line: 3 schemes
tags:
- Outbound outreach
- LinkedIn sourcing
- B2B SaaS
---
