---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: centers-for-disease-control-and-prevention-soda-v2-1-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention SODA v2.1 API
  slug: centers-for-disease-control-and-prevention-soda-v2-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-soda-v2-1-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-soda-v3-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention SODA v3 API
  slug: centers-for-disease-control-and-prevention-soda-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-soda-v3-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-app-notifications-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention App Notifications API
  slug: centers-for-disease-control-and-prevention-app-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-app-notifications-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-code-systems-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Code Systems API
  slug: centers-for-disease-control-and-prevention-code-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-code-systems-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-conditions-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Conditions API
  slug: centers-for-disease-control-and-prevention-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-conditions-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-configurations-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Configurations API
  slug: centers-for-disease-control-and-prevention-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-configurations-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-events-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Events API
  slug: centers-for-disease-control-and-prevention-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-events-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-query-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Query API
  slug: centers-for-disease-control-and-prevention-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-query-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-query-connector-api-openapi-3-0-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Query Connector API OpenAPI 3.0 API
  slug: centers-for-disease-control-and-prevention-query-connector-api-openapi-3-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-query-connector-api-openapi-3-0-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-releases-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Releases API
  slug: centers-for-disease-control-and-prevention-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-releases-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-simulator-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Simulator API
  slug: centers-for-disease-control-and-prevention-simulator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-simulator-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-tes-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention Tes API
  slug: centers-for-disease-control-and-prevention-tes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-tes-api-openapi.yml
- filename: centers-for-disease-control-and-prevention-user-api-openapi.yml
  format: yaml
  label: Centers for Disease Control and Prevention User API
  slug: centers-for-disease-control-and-prevention-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Centers For Disease Control And Prevention Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centers for Disease Control and Prevention secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Centers for Disease Control and Prevention
provider_slug: centers-for-disease-control-and-prevention
scheme_count: 1
schemes:
- description: 'Socrata application token. Anonymous use is allowed at throttled rates;

    an app token raises rate limits. May also be supplied as the

    $$app_token query parameter.'
  in: header
  name: appToken
  parameter: X-App-Token
  sources:
  - openapi/centers-for-disease-control-and-prevention-soda-v2-1-api-openapi.yml
  - openapi/centers-for-disease-control-and-prevention-soda-v3-api-openapi.yml
  type: apiKey
slug: centers-for-disease-control-and-prevention-authentication
source_filename: centers-for-disease-control-and-prevention-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/centers-for-disease-control-and-prevention-soda-v2-1-api-openapi.yml, openapi/centers-for-disease-control-and-prevention-soda-v3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: appToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  description: |-\n    Socrata application token. Anonymous use is allowed at throttled rates;\n    an app token raises rate limits. May also be supplied as the\n    $$app_token query parameter.\n  sources:\n  - openapi/centers-for-disease-control-and-prevention-soda-v2-1-api-openapi.yml\n  - openapi/centers-for-disease-control-and-prevention-soda-v3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/authentication/centers-for-disease-control-and-prevention-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Environmental Health
- Epidemiology
- Federal Government
- Healthcare
- Open Data
- Public Health
- Socrata
- Surveillance
- WONDER
---
