---
api_specs:
- filename: meltwater-account-management-api-openapi.yml
  format: yaml
  label: Meltwater Account Management API
  slug: meltwater-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-account-management-api-openapi.yml
- filename: meltwater-bring-your-own-content-byoc-api-openapi.yml
  format: yaml
  label: Meltwater Bring Your Own Content (BYOC) API
  slug: meltwater-bring-your-own-content-byoc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-bring-your-own-content-byoc-api-openapi.yml
- filename: meltwater-explore-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Analytics API
  slug: meltwater-explore-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-analytics-api-openapi.yml
- filename: meltwater-explore-assets-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Assets API
  slug: meltwater-explore-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-assets-api-openapi.yml
- filename: meltwater-explore-search-api-openapi.yml
  format: yaml
  label: Meltwater Explore+ Search API
  slug: meltwater-explore-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-explore-search-api-openapi.yml
- filename: meltwater-listening-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Listening Analytics API
  slug: meltwater-listening-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-analytics-api-openapi.yml
- filename: meltwater-listening-exports-api-openapi.yml
  format: yaml
  label: Meltwater Listening Exports API
  slug: meltwater-listening-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-exports-api-openapi.yml
- filename: meltwater-listening-search-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search API
  slug: meltwater-listening-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-api-openapi.yml
- filename: meltwater-listening-search-management-api-openapi.yml
  format: yaml
  label: Meltwater Listening Search Management API
  slug: meltwater-listening-search-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-search-management-api-openapi.yml
- filename: meltwater-listening-streaming-api-openapi.yml
  format: yaml
  label: Meltwater Listening Streaming API
  slug: meltwater-listening-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-listening-streaming-api-openapi.yml
- filename: meltwater-mira-api-api-openapi.yml
  format: yaml
  label: Meltwater Mira API API
  slug: meltwater-mira-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-mira-api-api-openapi.yml
- filename: meltwater-owned-analytics-api-openapi.yml
  format: yaml
  label: Meltwater Owned Analytics API
  slug: meltwater-owned-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-owned-analytics-api-openapi.yml
- filename: meltwater-api-v4-openapi.yml
  format: yaml
  label: Meltwater API v4
  slug: meltwater-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/openapi/meltwater-api-v4-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Meltwater Trust Center
name_suffix: Trust Center
overview: Meltwater maintains a public trust center covering its security and compliance posture.
provider_name: Meltwater
provider_slug: meltwater
slug: meltwater-trust-center
source_filename: meltwater-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.meltwater.com/\nplatform: Vanta Trust Center\ncertifications: []\nnote: >-\n  trust.meltwater.com returns HTTP 200 with the title \"Meltwater Trust Center\" and is a\n  Vanta-hosted trust page, so the trust center genuinely exists. The certification list is\n  rendered client-side by the Vanta app and the underlying API (api.vanta.com) answers 401\n  anonymously, so no named certification could be read without fabricating it - the empty\n  list means \"checked, not machine-readable\", not \"none held\". No `Compliance` pointer is\n  emitted for that reason.\nevidence:\n  - source: https://trust.meltwater.com/\n    status: 200\n    kind: vanta trust center (JS-rendered)\n    keywords: [Trust, Security, Compliance]\nrelated:\n  - type: data-provider compliance changes\n    url: https://developer.meltwater.com/help/compliance\n    note: >-\n      Meltwater's developer portal also publishes a Compliance page,\
  \ but it documents API field\n      removals made to stay within X/Twitter and YouTube terms of service - it is not a security\n      certification statement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meltwater/refs/heads/main/security/meltwater-trust-center.yml
summary_line: trust center published
tags:
- Media Monitoring
- Social Listening
- PR Analytics
- Brand Intelligence
- News API
- Social Analytics
- Media Intelligence
trust_url: https://trust.meltwater.com/
---
