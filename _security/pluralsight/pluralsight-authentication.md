---
api_key_in: []
api_specs:
- filename: pluralsight-catalog-api-openapi.yml
  format: yaml
  label: Pluralsight Catalog API
  slug: pluralsight-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-catalog-api-openapi.yml
- filename: pluralsight-coding-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Coding Metrics API
  slug: pluralsight-coding-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-coding-metrics-api-openapi.yml
- filename: pluralsight-collaboration-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Collaboration Metrics API
  slug: pluralsight-collaboration-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-collaboration-metrics-api-openapi.yml
- filename: pluralsight-commits-api-openapi.yml
  format: yaml
  label: Pluralsight Commits API
  slug: pluralsight-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-commits-api-openapi.yml
- filename: pluralsight-dora-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight DORA Metrics API
  slug: pluralsight-dora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-dora-metrics-api-openapi.yml
- filename: pluralsight-graphql-api-openapi.yml
  format: yaml
  label: Pluralsight GraphQL API
  slug: pluralsight-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-graphql-api-openapi.yml
- filename: pluralsight-integrations-api-openapi.yml
  format: yaml
  label: Pluralsight Integrations API
  slug: pluralsight-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-integrations-api-openapi.yml
- filename: pluralsight-licensing-api-openapi.yml
  format: yaml
  label: Pluralsight Licensing API
  slug: pluralsight-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-licensing-api-openapi.yml
- filename: pluralsight-pull-requests-api-openapi.yml
  format: yaml
  label: Pluralsight Pull Requests API
  slug: pluralsight-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-pull-requests-api-openapi.yml
- filename: pluralsight-reports-api-openapi.yml
  format: yaml
  label: Pluralsight Reports API
  slug: pluralsight-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-reports-api-openapi.yml
- filename: pluralsight-repos-api-openapi.yml
  format: yaml
  label: Pluralsight Repos API
  slug: pluralsight-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-repos-api-openapi.yml
- filename: pluralsight-teams-api-openapi.yml
  format: yaml
  label: Pluralsight Teams API
  slug: pluralsight-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-teams-api-openapi.yml
- filename: pluralsight-tickets-api-openapi.yml
  format: yaml
  label: Pluralsight Tickets API
  slug: pluralsight-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-tickets-api-openapi.yml
- filename: pluralsight-users-api-openapi.yml
  format: yaml
  label: Pluralsight Users API
  slug: pluralsight-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pluralsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pluralsight secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pluralsight
provider_slug: pluralsight
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/channels.yml
  - openapi/content-catalog.yml
  - openapi/content-progress.yml
  - openapi/content-slug.yml
  - openapi/course-catalog.yml
  - openapi/course-daily-usage.yml
  - openapi/course-progress.yml
  - openapi/flow-coding-metrics.yml
  - openapi/flow-collaboration-metrics.yml
  - openapi/flow-commits.yml
  - openapi/flow-dora-metrics.yml
  - openapi/flow-integrations.yml
  - openapi/flow-pull-requests.yml
  - openapi/flow-repos.yml
  - openapi/flow-teams.yml
  - openapi/flow-tickets.yml
  - openapi/flow-users.yml
  - openapi/labs.yml
  - openapi/learning-paths.yml
  - openapi/licensing-rest.yml
  - openapi/plan-info.yml
  - openapi/practice-exams.yml
  - openapi/programs.yml
  - openapi/reports-rest.yml
  - openapi/role-iq.yml
  - openapi/skills-assessment.yml
  - openapi/tags.yml
  - openapi/teams.yml
  - openapi/user-management.yml
  type: http
slug: pluralsight-authentication
source_filename: pluralsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/channels.yml, openapi/content-catalog.yml, openapi/content-progress.yml, openapi/content-slug.yml,\n  openapi/course-catalog.yml, openapi/course-daily-usage.yml, openapi/course-progress.yml, openapi/flow-coding-metrics.yml,\n  openapi/flow-collaboration-metrics.yml, openapi/flow-commits.yml, openapi/flow-dora-metrics.yml,\n  openapi/flow-integrations.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/channels.yml\n  - openapi/content-catalog.yml\n  - openapi/content-progress.yml\n  - openapi/content-slug.yml\n  - openapi/course-catalog.yml\n  - openapi/course-daily-usage.yml\n  - openapi/course-progress.yml\n  - openapi/flow-coding-metrics.yml\n  - openapi/flow-collaboration-metrics.yml\n  - openapi/flow-commits.yml\n  - openapi/flow-dora-metrics.yml\n  - openapi/flow-integrations.yml\n  - openapi/flow-pull-requests.yml\n \
  \ - openapi/flow-repos.yml\n  - openapi/flow-teams.yml\n  - openapi/flow-tickets.yml\n  - openapi/flow-users.yml\n  - openapi/labs.yml\n  - openapi/learning-paths.yml\n  - openapi/licensing-rest.yml\n  - openapi/plan-info.yml\n  - openapi/practice-exams.yml\n  - openapi/programs.yml\n  - openapi/reports-rest.yml\n  - openapi/role-iq.yml\n  - openapi/skills-assessment.yml\n  - openapi/tags.yml\n  - openapi/teams.yml\n  - openapi/user-management.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/authentication/pluralsight-authentication.yml
summary_line: http · 1 scheme
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
---
