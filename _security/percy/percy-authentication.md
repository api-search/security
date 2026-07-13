---
api_key_in: []
api_specs:
- filename: percy-openapi.yml
  format: yaml
  label: Percy Builds API
  slug: percy-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/percy/refs/heads/main/openapi/percy-openapi.yml
- filename: percy-openapi.yml
  format: yaml
  label: Percy Snapshots API
  slug: percy-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/percy/refs/heads/main/openapi/percy-openapi.yml
- filename: percy-openapi.yml
  format: yaml
  label: Percy Projects API
  slug: percy-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/percy/refs/heads/main/openapi/percy-openapi.yml
- filename: percy-openapi.yml
  format: yaml
  label: Percy Visual Git API
  slug: percy-visual-git-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/percy/refs/heads/main/openapi/percy-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: sourced
name: Percy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Percy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Percy
provider_slug: percy
scheme_count: 2
schemes:
- description: 'Per-project token used for read operations (list/get on projects, builds, and snapshots, and all Visual Git calls). Passed in the Authorization header using Percy''s token scheme - literally `Authorization: Token token=<PROJECT_TOKEN>`. The project token (PERCY_TOKEN) is the same value the Percy CLI/SDK uses to upload snapshots during a build; find it in the project settings in the Percy / BrowserStack dashboard.'
  headerName: Authorization
  in: header
  name: projectToken
  sources:
  - https://www.browserstack.com/docs/percy/api-reference/builds
  - https://www.browserstack.com/docs/percy/api-reference/snapshots
  type: apiKey
- description: BrowserStack HTTP Basic auth (base64 of username:accesskey), required for review and write operations - approving/unapproving/rejecting a build, manually failing or deleting a build, and creating or updating a project. Uses your BrowserStack username and access key.
  name: browserstackBasic
  scheme: basic
  sources:
  - https://www.browserstack.com/docs/percy/api-reference/builds
  - https://www.browserstack.com/docs/percy/api-reference/projects
  type: http
slug: percy-authentication
source_filename: percy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: sourced\nsource: BrowserStack Percy API reference (builds, snapshots, projects, visual-git)\nsummary:\n  types:\n  - apiKey\n  - http\nschemes:\n- name: projectToken\n  type: apiKey\n  in: header\n  headerName: Authorization\n  description: >-\n    Per-project token used for read operations (list/get on projects, builds, and\n    snapshots, and all Visual Git calls). Passed in the Authorization header using\n    Percy's token scheme - literally `Authorization: Token token=<PROJECT_TOKEN>`.\n    The project token (PERCY_TOKEN) is the same value the Percy CLI/SDK uses to\n    upload snapshots during a build; find it in the project settings in the Percy /\n    BrowserStack dashboard.\n  sources:\n  - https://www.browserstack.com/docs/percy/api-reference/builds\n  - https://www.browserstack.com/docs/percy/api-reference/snapshots\n- name: browserstackBasic\n  type: http\n  scheme: basic\n  description: >-\n    BrowserStack HTTP Basic auth (base64\
  \ of username:accesskey), required for review\n    and write operations - approving/unapproving/rejecting a build, manually failing\n    or deleting a build, and creating or updating a project. Uses your BrowserStack\n    username and access key.\n  sources:\n  - https://www.browserstack.com/docs/percy/api-reference/builds\n  - https://www.browserstack.com/docs/percy/api-reference/projects\nnotes: >-\n  Snapshot capture and upload during a build is performed by the open-source Percy\n  CLI/SDK using the same PERCY_TOKEN project token; that upload path is SDK-internal\n  and is not part of the documented public REST reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/percy/refs/heads/main/authentication/percy-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Visual Testing
- Visual Regression
- Screenshots
- QA
- Testing
- CI/CD
- BrowserStack
---
