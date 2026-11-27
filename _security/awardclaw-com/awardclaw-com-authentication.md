---
anonymous_access: false
api_key_in: []
api_specs:
- filename: awardclaw-com-availability-api-openapi.yml
  format: yaml
  label: AwardClaw Availability API
  slug: awardclaw-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-availability-api-openapi.yml
- filename: awardclaw-com-briefing-api-openapi.yml
  format: yaml
  label: AwardClaw Briefing API
  slug: awardclaw-com-briefing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-briefing-api-openapi.yml
- filename: awardclaw-com-cards-api-openapi.yml
  format: yaml
  label: AwardClaw Cards API
  slug: awardclaw-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-cards-api-openapi.yml
- filename: awardclaw-com-drops-api-openapi.yml
  format: yaml
  label: AwardClaw Drops API
  slug: awardclaw-com-drops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-drops-api-openapi.yml
- filename: awardclaw-com-me-api-openapi.yml
  format: yaml
  label: AwardClaw Me API
  slug: awardclaw-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-me-api-openapi.yml
- filename: awardclaw-com-news-api-openapi.yml
  format: yaml
  label: AwardClaw News API
  slug: awardclaw-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-news-api-openapi.yml
- filename: awardclaw-com-watches-api-openapi.yml
  format: yaml
  label: AwardClaw Watches API
  slug: awardclaw-com-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-watches-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AwardClaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: AwardClaw secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AwardClaw
provider_slug: awardclaw-com
scheme_count: 1
schemes:
- description: ac_live_ key from awardclaw.com/dashboard/agents
  name: bearer
  scheme: bearer
  sources:
  - openapi/awardclaw-com-openapi.json
  type: http
slug: awardclaw-com-authentication
source_filename: awardclaw-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/awardclaw-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: ac_live_ key from awardclaw.com/dashboard/agents\n  sources:\n  - openapi/awardclaw-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/awardclaw-com/authentication/awardclaw-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Travel
- Awards
- Airlines
- Flight Deals
- Automation
- Newsletters
---
