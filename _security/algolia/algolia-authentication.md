---
api_key_in:
- header
api_specs:
- filename: algolia-search-api-openapi.yml
  format: yaml
  label: Algolia Search API
  slug: algolia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-search-api-openapi.yml
- filename: algolia-insights-api-openapi.yml
  format: yaml
  label: Algolia Insights API
  slug: algolia-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-insights-api-openapi.yml
- filename: algolia-recommend-api-openapi.yml
  format: yaml
  label: Algolia Recommend API
  slug: algolia-recommend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-recommend-api-openapi.yml
- filename: algolia-analytics-api-openapi.yml
  format: yaml
  label: Algolia Analytics API
  slug: algolia-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-analytics-api-openapi.yml
- filename: algolia-abtesting-v3-api-openapi.yml
  format: yaml
  label: Algolia A/B Testing API
  slug: algolia-ab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-abtesting-v3-api-openapi.yml
- filename: algolia-personalization-api-openapi.yml
  format: yaml
  label: Algolia Personalization API
  slug: algolia-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-personalization-api-openapi.yml
- filename: algolia-advanced-personalization-api-openapi.yml
  format: yaml
  label: Algolia Advanced Personalization API
  slug: algolia-advanced-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-advanced-personalization-api-openapi.yml
- filename: algolia-crawler-api-openapi.yml
  format: yaml
  label: Algolia Crawler API
  slug: algolia-crawler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-crawler-api-openapi.yml
- filename: algolia-ingestion-api-openapi.yml
  format: yaml
  label: Algolia Ingestion API
  slug: algolia-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-ingestion-api-openapi.yml
- filename: algolia-query-suggestions-api-openapi.yml
  format: yaml
  label: Algolia Query Suggestions API
  slug: algolia-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-query-suggestions-api-openapi.yml
- filename: algolia-composition-api-openapi.yml
  format: yaml
  label: Algolia Composition API
  slug: algolia-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-composition-api-openapi.yml
- filename: algolia-agent-studio-api-openapi.yml
  format: yaml
  label: Algolia Agent Studio API
  slug: algolia-agent-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-agent-studio-api-openapi.yml
- filename: algolia-monitoring-api-openapi.yml
  format: yaml
  label: Algolia Monitoring API
  slug: algolia-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-monitoring-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Algolia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algolia secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Algolia
provider_slug: algolia
scheme_count: 5
schemes:
- description: Your Algolia application ID.
  in: header
  name: appId
  parameter: x-algolia-application-id
  sources:
  - openapi/algolia-abtesting-openapi.yml
  - openapi/algolia-abtesting-v3-openapi.yml
  - openapi/algolia-advanced-personalization-openapi.yml
  - openapi/algolia-agent-studio-openapi.yml
  - openapi/algolia-algoliasearch-openapi.yml
  - openapi/algolia-composition-openapi.yml
  - openapi/algolia-ingestion-openapi.yml
  - openapi/algolia-insights-openapi.yml
  - openapi/algolia-personalization-openapi.yml
  - openapi/algolia-query-suggestions-openapi.yml
  - openapi/algolia-recommend-openapi.yml
  - openapi/algolia-search-openapi.yml
  type: apiKey
- description: 'Your Algolia API key with the necessary permissions to make the request.

    Permissions are controlled through access control lists (ACL) and access restrictions.

    The required ACL to make a request is listed in each endpoint''s reference.'
  in: header
  name: apiKey
  parameter: x-algolia-api-key
  sources:
  - openapi/algolia-abtesting-openapi.yml
  - openapi/algolia-abtesting-v3-openapi.yml
  - openapi/algolia-advanced-personalization-openapi.yml
  - openapi/algolia-agent-studio-openapi.yml
  - openapi/algolia-algoliasearch-openapi.yml
  - openapi/algolia-composition-openapi.yml
  - openapi/algolia-ingestion-openapi.yml
  - openapi/algolia-insights-openapi.yml
  - openapi/algolia-personalization-openapi.yml
  - openapi/algolia-query-suggestions-openapi.yml
  - openapi/algolia-recommend-openapi.yml
  - openapi/algolia-search-openapi.yml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/algolia-crawler-openapi.yml
  type: http
- description: Your Algolia application ID.
  in: header
  name: appId
  parameter: X-Algolia-Application-Id
  sources:
  - openapi/algolia-monitoring-openapi.yml
  type: apiKey
- description: Your Algolia Monitoring API key.
  in: header
  name: apiKey
  parameter: X-Algolia-API-Key
  sources:
  - openapi/algolia-monitoring-openapi.yml
  type: apiKey
slug: algolia-authentication
source_filename: algolia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: derived\nsource: openapi/algolia-abtesting-openapi.yml, openapi/algolia-abtesting-v3-openapi.yml, openapi/algolia-advanced-personalization-openapi.yml,\n  openapi/algolia-agent-studio-openapi.yml, openapi/algolia-algoliasearch-openapi.yml, openapi/algolia-composition-openapi.yml,\n  openapi/algolia-crawler-openapi.yml, openapi/algolia-ingestion-openapi.yml, openapi/algolia-insights-openapi.yml,\n  openapi/algolia-monitoring-openapi.yml, openapi/algolia-personalization-openapi.yml, openapi/algolia-query-suggestions-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: appId\n  type: apiKey\n  in: header\n  parameter: x-algolia-application-id\n  description: Your Algolia application ID.\n  sources:\n  - openapi/algolia-abtesting-openapi.yml\n  - openapi/algolia-abtesting-v3-openapi.yml\n  - openapi/algolia-advanced-personalization-openapi.yml\n  - openapi/algolia-agent-studio-openapi.yml\n \
  \ - openapi/algolia-algoliasearch-openapi.yml\n  - openapi/algolia-composition-openapi.yml\n  - openapi/algolia-ingestion-openapi.yml\n  - openapi/algolia-insights-openapi.yml\n  - openapi/algolia-personalization-openapi.yml\n  - openapi/algolia-query-suggestions-openapi.yml\n  - openapi/algolia-recommend-openapi.yml\n  - openapi/algolia-search-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-algolia-api-key\n  description: |-\n    Your Algolia API key with the necessary permissions to make the request.\n    Permissions are controlled through access control lists (ACL) and access restrictions.\n    The required ACL to make a request is listed in each endpoint's reference.\n  sources:\n  - openapi/algolia-abtesting-openapi.yml\n  - openapi/algolia-abtesting-v3-openapi.yml\n  - openapi/algolia-advanced-personalization-openapi.yml\n  - openapi/algolia-agent-studio-openapi.yml\n  - openapi/algolia-algoliasearch-openapi.yml\n  - openapi/algolia-composition-openapi.yml\n\
  \  - openapi/algolia-ingestion-openapi.yml\n  - openapi/algolia-insights-openapi.yml\n  - openapi/algolia-personalization-openapi.yml\n  - openapi/algolia-query-suggestions-openapi.yml\n  - openapi/algolia-recommend-openapi.yml\n  - openapi/algolia-search-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/algolia-crawler-openapi.yml\n- name: appId\n  type: apiKey\n  in: header\n  parameter: X-Algolia-Application-Id\n  description: Your Algolia application ID.\n  sources:\n  - openapi/algolia-monitoring-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Algolia-API-Key\n  description: Your Algolia Monitoring API key.\n  sources:\n  - openapi/algolia-monitoring-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/authentication/algolia-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Search
- Discovery
- Recommendations
- Personalization
- Analytics
- E-Commerce
---
