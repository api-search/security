---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justgains-com-auth-api-openapi.yml
  format: yaml
  label: JustGains Auth API
  slug: justgains-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-auth-api-openapi.yml
- filename: justgains-com-authen-api-openapi.yml
  format: yaml
  label: JustGains Authen API
  slug: justgains-com-authen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-authen-api-openapi.yml
- filename: justgains-com-creatorprofiles-api-openapi.yml
  format: yaml
  label: JustGains Creator Profiles API
  slug: justgains-com-creatorprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-creatorprofiles-api-openapi.yml
- filename: justgains-com-equipment-api-openapi.yml
  format: yaml
  label: JustGains Equipment API
  slug: justgains-com-equipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-equipment-api-openapi.yml
- filename: justgains-com-equipmentgroups-api-openapi.yml
  format: yaml
  label: JustGains Equipment Groups API
  slug: justgains-com-equipmentgroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-equipmentgroups-api-openapi.yml
- filename: justgains-com-exercise-api-openapi.yml
  format: yaml
  label: JustGains Exercise API
  slug: justgains-com-exercise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exercise-api-openapi.yml
- filename: justgains-com-exercisecategory-api-openapi.yml
  format: yaml
  label: JustGains Exercise Category API
  slug: justgains-com-exercisecategory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exercisecategory-api-openapi.yml
- filename: justgains-com-exercisedraft-api-openapi.yml
  format: yaml
  label: JustGains Exercise Draft API
  slug: justgains-com-exercisedraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exercisedraft-api-openapi.yml
- filename: justgains-com-exerciseinstruction-api-openapi.yml
  format: yaml
  label: JustGains Exercise Instruction API
  slug: justgains-com-exerciseinstruction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exerciseinstruction-api-openapi.yml
- filename: justgains-com-exercisemetric-api-openapi.yml
  format: yaml
  label: JustGains Exercise Metric API
  slug: justgains-com-exercisemetric-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exercisemetric-api-openapi.yml
- filename: justgains-com-exercisevideo-api-openapi.yml
  format: yaml
  label: JustGains Exercise Video API
  slug: justgains-com-exercisevideo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-exercisevideo-api-openapi.yml
- filename: justgains-com-justgains-api-api-openapi.yml
  format: yaml
  label: JustGains Just Gains API
  slug: justgains-com-justgains-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-justgains-api-api-openapi.yml
- filename: justgains-com-locale-api-openapi.yml
  format: yaml
  label: JustGains Locale API
  slug: justgains-com-locale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-locale-api-openapi.yml
- filename: justgains-com-mediaasset-api-openapi.yml
  format: yaml
  label: JustGains Media Asset API
  slug: justgains-com-mediaasset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-mediaasset-api-openapi.yml
- filename: justgains-com-muscle-api-openapi.yml
  format: yaml
  label: JustGains Muscle API
  slug: justgains-com-muscle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-muscle-api-openapi.yml
- filename: justgains-com-musclegroup-api-openapi.yml
  format: yaml
  label: JustGains Muscle Group API
  slug: justgains-com-musclegroup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-musclegroup-api-openapi.yml
- filename: justgains-com-publishedstatuses-api-openapi.yml
  format: yaml
  label: JustGains Published Statuses API
  slug: justgains-com-publishedstatuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-publishedstatuses-api-openapi.yml
- filename: justgains-com-user-api-openapi.yml
  format: yaml
  label: JustGains User API
  slug: justgains-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-user-api-openapi.yml
- filename: justgains-com-workout-api-openapi.yml
  format: yaml
  label: JustGains Workout API
  slug: justgains-com-workout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justgains-com/openapi/justgains-com-workout-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustGains Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustGains secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustGains
provider_slug: justgains-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Put **_ONLY_** your JWT Bearer token on the textbox below!
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/justgains-com-openapi.json
  type: http
slug: justgains-com-authentication
source_filename: justgains-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justgains-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Put **_ONLY_** your JWT Bearer token on the textbox below!\n  sources:\n  - openapi/justgains-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/justgains-com/authentication/justgains-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Fitness
- Health
- Workouts
- Nutrition
- Platform
---
