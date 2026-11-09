---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: bokendell-com-activity-api-openapi.yml
  format: yaml
  label: Bo Kendell Activity API
  slug: bokendell-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-activity-api-openapi.yml
- filename: bokendell-com-ai-api-openapi.yml
  format: yaml
  label: Bo Kendell AI API
  slug: bokendell-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-ai-api-openapi.yml
- filename: bokendell-com-contacts-api-openapi.yml
  format: yaml
  label: Bo Kendell Contacts API
  slug: bokendell-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-contacts-api-openapi.yml
- filename: bokendell-com-events-api-openapi.yml
  format: yaml
  label: Bo Kendell Events API
  slug: bokendell-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-events-api-openapi.yml
- filename: bokendell-com-health-api-openapi.yml
  format: yaml
  label: Bo Kendell Health API
  slug: bokendell-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-health-api-openapi.yml
- filename: bokendell-com-profile-api-openapi.yml
  format: yaml
  label: Bo Kendell Profile API
  slug: bokendell-com-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-profile-api-openapi.yml
- filename: bokendell-com-projects-api-openapi.yml
  format: yaml
  label: Bo Kendell Projects API
  slug: bokendell-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-projects-api-openapi.yml
- filename: bokendell-com-resume-api-openapi.yml
  format: yaml
  label: Bo Kendell Resume API
  slug: bokendell-com-resume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-resume-api-openapi.yml
- filename: bokendell-com-social-links-api-openapi.yml
  format: yaml
  label: Bo Kendell Social Links API
  slug: bokendell-com-social-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-social-links-api-openapi.yml
- filename: bokendell-com-tags-api-openapi.yml
  format: yaml
  label: Bo Kendell Tags API
  slug: bokendell-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-tags-api-openapi.yml
- filename: bokendell-com-technologies-api-openapi.yml
  format: yaml
  label: Bo Kendell Technologies API
  slug: bokendell-com-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-technologies-api-openapi.yml
- filename: bokendell-com-writing-api-openapi.yml
  format: yaml
  label: Bo Kendell Writing API
  slug: bokendell-com-writing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bokendell-com/openapi/bokendell-com-writing-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bokendell Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bo Kendell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bo Kendell
provider_slug: bokendell-com
scheme_count: 1
schemes:
- description: Better Auth session cookie
  in: cookie
  name: cookieAuth
  parameter: better-auth.session_token
  sources:
  - openapi/bokendell-com-openapi.json
  type: apiKey
slug: bokendell-com-authentication
source_filename: bokendell-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bokendell-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: better-auth.session_token\n  description: Better Auth session cookie\n  sources:\n  - openapi/bokendell-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bokendell-com/authentication/bokendell-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Software Engineer
- Backend
- Artificial Intelligence
- OpenAPI
- MCP
---
