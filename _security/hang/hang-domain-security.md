---
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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hang.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hang.xyz
  spf: true
hosts:
- cert_expires: Oct 16 19:42:49 2026 GMT
  host: www.hang.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:29:19 2026 GMT
  host: docs.hang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:33:46 2026 GMT
  host: loyalty.hang.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hang, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hang
provider_slug: hang
slug: hang-domain-security
source_filename: hang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:29:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: loyalty.hang.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:33:46 2026 GMT\n  hsts: null\ndomains:\n- domain: hang.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hang.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hang/refs/heads/main/security/hang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Loyalty
- Rewards
- Membership
- Customer Engagement
- Marketing
- Restaurant
- Point-of-Sale
- Webhook
---
