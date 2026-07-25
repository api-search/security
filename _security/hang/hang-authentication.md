---
api_key_in:
- header
api_specs:
- filename: hang-activities-api-openapi.yml
  format: yaml
  label: Hang Activities API
  slug: hang-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-activities-api-openapi.yml
- filename: hang-loot-box-reward-choices-api-openapi.yml
  format: yaml
  label: Hang Loot Box Reward Choices API
  slug: hang-loot-box-reward-choices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-loot-box-reward-choices-api-openapi.yml
- filename: hang-loot-box-reward-probabilities-api-openapi.yml
  format: yaml
  label: Hang Loot box reward probabilities API
  slug: hang-loot-box-reward-probabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-loot-box-reward-probabilities-api-openapi.yml
- filename: hang-loot-boxes-api-openapi.yml
  format: yaml
  label: Hang Loot Boxes API
  slug: hang-loot-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-loot-boxes-api-openapi.yml
- filename: hang-member-actions-api-openapi.yml
  format: yaml
  label: Hang Member Actions API
  slug: hang-member-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-member-actions-api-openapi.yml
- filename: hang-memberships-api-openapi.yml
  format: yaml
  label: Hang Memberships API
  slug: hang-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-memberships-api-openapi.yml
- filename: hang-program-memberships-api-openapi.yml
  format: yaml
  label: Hang Program memberships API
  slug: hang-program-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-program-memberships-api-openapi.yml
- filename: hang-program-tiers-api-openapi.yml
  format: yaml
  label: Hang Program Tiers API
  slug: hang-program-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-program-tiers-api-openapi.yml
- filename: hang-programmembershippuzzles-api-openapi.yml
  format: yaml
  label: Hang ProgramMembershipPuzzles API
  slug: hang-programmembershippuzzles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-programmembershippuzzles-api-openapi.yml
- filename: hang-programs-api-openapi.yml
  format: yaml
  label: Hang Programs API
  slug: hang-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-programs-api-openapi.yml
- filename: hang-puzzles-api-openapi.yml
  format: yaml
  label: Hang Puzzles API
  slug: hang-puzzles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-puzzles-api-openapi.yml
- filename: hang-quests-api-openapi.yml
  format: yaml
  label: Hang Quests API
  slug: hang-quests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-quests-api-openapi.yml
- filename: hang-redemptions-api-openapi.yml
  format: yaml
  label: Hang Redemptions API
  slug: hang-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-redemptions-api-openapi.yml
- filename: hang-rewards-api-openapi.yml
  format: yaml
  label: Hang Rewards API
  slug: hang-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-rewards-api-openapi.yml
- filename: hang-tokenizedrewards-api-openapi.yml
  format: yaml
  label: Hang TokenizedRewards API
  slug: hang-tokenizedrewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-tokenizedrewards-api-openapi.yml
- filename: hang-tokens-api-openapi.yml
  format: yaml
  label: Hang Tokens API
  slug: hang-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-tokens-api-openapi.yml
- filename: hang-users-api-openapi.yml
  format: yaml
  label: Hang Users API
  slug: hang-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-users-api-openapi.yml
- filename: hang-wallet-integration-api-openapi.yml
  format: yaml
  label: Hang Wallet Integration API
  slug: hang-wallet-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/openapi/hang-wallet-integration-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hang Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hang secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hang
provider_slug: hang
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/hang-partner-api-openapi.yml
  type: apiKey
slug: hang-authentication
source_filename: hang-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hang-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/hang-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/authentication/hang-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Loyalty
- Rewards
- Membership
- Customer Engagement
- Marketing
- Restaurants
- Point of Sale
- Webhooks
---
