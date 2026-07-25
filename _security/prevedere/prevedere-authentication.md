---
api_key_in:
- query
api_specs:
- filename: prevedere-alert-api-openapi.yml
  format: yaml
  label: Prevedere Alert API
  slug: prevedere-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-alert-api-openapi.yml
- filename: prevedere-alertdefinition-api-openapi.yml
  format: yaml
  label: Prevedere AlertDefinition API
  slug: prevedere-alertdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-alertdefinition-api-openapi.yml
- filename: prevedere-analysisjob-api-openapi.yml
  format: yaml
  label: Prevedere AnalysisJob API
  slug: prevedere-analysisjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-analysisjob-api-openapi.yml
- filename: prevedere-componentcontributionoverridevalues-api-openapi.yml
  format: yaml
  label: Prevedere ComponentContributionOverrideValues API
  slug: prevedere-componentcontributionoverridevalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-componentcontributionoverridevalues-api-openapi.yml
- filename: prevedere-context-api-openapi.yml
  format: yaml
  label: Prevedere Context API
  slug: prevedere-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-context-api-openapi.yml
- filename: prevedere-dataintegration-api-openapi.yml
  format: yaml
  label: Prevedere DataIntegration API
  slug: prevedere-dataintegration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-dataintegration-api-openapi.yml
- filename: prevedere-discoverjob-api-openapi.yml
  format: yaml
  label: Prevedere DiscoverJob API
  slug: prevedere-discoverjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-discoverjob-api-openapi.yml
- filename: prevedere-enumeration-api-openapi.yml
  format: yaml
  label: Prevedere Enumeration API
  slug: prevedere-enumeration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-enumeration-api-openapi.yml
- filename: prevedere-favorites-api-openapi.yml
  format: yaml
  label: Prevedere Favorites API
  slug: prevedere-favorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-favorites-api-openapi.yml
- filename: prevedere-forecastmodel-api-openapi.yml
  format: yaml
  label: Prevedere ForecastModel API
  slug: prevedere-forecastmodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-forecastmodel-api-openapi.yml
- filename: prevedere-forecastmodelhistory-api-openapi.yml
  format: yaml
  label: Prevedere ForecastModelHistory API
  slug: prevedere-forecastmodelhistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-forecastmodelhistory-api-openapi.yml
- filename: prevedere-forecastsummary-api-openapi.yml
  format: yaml
  label: Prevedere ForecastSummary API
  slug: prevedere-forecastsummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-forecastsummary-api-openapi.yml
- filename: prevedere-indicator-api-openapi.yml
  format: yaml
  label: Prevedere Indicator API
  slug: prevedere-indicator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-indicator-api-openapi.yml
- filename: prevedere-provider-api-openapi.yml
  format: yaml
  label: Prevedere Provider API
  slug: prevedere-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-provider-api-openapi.yml
- filename: prevedere-scenario-api-openapi.yml
  format: yaml
  label: Prevedere Scenario API
  slug: prevedere-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-scenario-api-openapi.yml
- filename: prevedere-tag-api-openapi.yml
  format: yaml
  label: Prevedere Tag API
  slug: prevedere-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-tag-api-openapi.yml
- filename: prevedere-test-api-openapi.yml
  format: yaml
  label: Prevedere Test API
  slug: prevedere-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-test-api-openapi.yml
- filename: prevedere-usercontext-api-openapi.yml
  format: yaml
  label: Prevedere UserContext API
  slug: prevedere-usercontext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-usercontext-api-openapi.yml
- filename: prevedere-workbench-api-openapi.yml
  format: yaml
  label: Prevedere Workbench API
  slug: prevedere-workbench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/openapi/prevedere-workbench-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prevedere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prevedere secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prevedere
provider_slug: prevedere
scheme_count: 1
schemes:
- in: query
  name: api key
  parameter: ApiKey
  sources:
  - openapi/prevedere-openapi-original.json
  type: apiKey
slug: prevedere-authentication
source_filename: prevedere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prevedere-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api key\n  type: apiKey\n  in: query\n  parameter: ApiKey\n  sources:\n  - openapi/prevedere-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prevedere/refs/heads/main/authentication/prevedere-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Economic Forecasting
- Predictive Analytics
- Demand Planning
- Financial Planning
- Macroeconomic Data
- Indicators
- Time Series
- Data Integration
- Machine Learning
---
