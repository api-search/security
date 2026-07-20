---
api_key_in: []
api_specs:
- filename: gradle-develocity-openapi.yaml
  format: yaml
  label: Develocity API
  slug: develocity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradle/refs/heads/main/openapi/gradle-develocity-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gradle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gradle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gradle
provider_slug: gradle
scheme_count: 1
schemes:
- bearerFormat: Bearer <<Develocity Access Key or Token>>
  description: "All requests require a Develocity access key or token as a bearer token. \nGiven an access key of `l3an7wk3j4ze5v4mi7rvgjf2p7g44nvlswg4cpvdonjs7rzd4kmq`, the required header is `Authorization: Bearer [example key]`.\n\nPlease consult the [Develocity API User Manual](https://gradle.com/help/api-access-control) for guidance on how to provision access keys or token"
  name: DevelocityAccessKeyOrToken
  scheme: bearer
  sources:
  - openapi/gradle-develocity-openapi.yaml
  type: http
slug: gradle-authentication
source_filename: gradle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gradle-develocity-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: DevelocityAccessKeyOrToken\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer <<Develocity Access Key or Token>>\n  description: \"All requests require a Develocity access key or token as a bearer token. \\n\\\n    Given an access key of `l3an7wk3j4ze5v4mi7rvgjf2p7g44nvlswg4cpvdonjs7rzd4kmq`, the required\\\n    \\ header is `Authorization: Bearer [example key]`.\\n\\\n    \\nPlease consult the [Develocity API User Manual](https://gradle.com/help/api-access-control)\\\n    \\ for guidance on how to provision access keys or token\"\n  sources:\n  - openapi/gradle-develocity-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradle/refs/heads/main/authentication/gradle-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Build Automation
- Developer Productivity
- CI/CD
- Build Analytics
- Testing
- DevOps
- Java
- Build Cache
---
