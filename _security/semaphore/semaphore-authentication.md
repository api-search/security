---
api_key_in: []
api_specs:
- filename: semaphore-dashboards-api-openapi.yml
  format: yaml
  label: Semaphore Dashboards API
  slug: semaphore-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-dashboards-api-openapi.yml
- filename: semaphore-deploymenttargets-api-openapi.yml
  format: yaml
  label: Semaphore DeploymentTargets API
  slug: semaphore-deploymenttargets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-deploymenttargets-api-openapi.yml
- filename: semaphore-notifications-api-openapi.yml
  format: yaml
  label: Semaphore Notifications API
  slug: semaphore-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-notifications-api-openapi.yml
- filename: semaphore-pipelines-api-openapi.yml
  format: yaml
  label: Semaphore Pipelines API
  slug: semaphore-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-pipelines-api-openapi.yml
- filename: semaphore-projects-api-openapi.yml
  format: yaml
  label: Semaphore Projects API
  slug: semaphore-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-projects-api-openapi.yml
- filename: semaphore-projectsecrets-api-openapi.yml
  format: yaml
  label: Semaphore ProjectSecrets API
  slug: semaphore-projectsecrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-projectsecrets-api-openapi.yml
- filename: semaphore-secrets-api-openapi.yml
  format: yaml
  label: Semaphore Secrets API
  slug: semaphore-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-secrets-api-openapi.yml
- filename: semaphore-selfhostedagents-api-openapi.yml
  format: yaml
  label: Semaphore SelfHostedAgents API
  slug: semaphore-selfhostedagents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-selfhostedagents-api-openapi.yml
- filename: semaphore-selfhostedagenttypes-api-openapi.yml
  format: yaml
  label: Semaphore SelfHostedAgentTypes API
  slug: semaphore-selfhostedagenttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-selfhostedagenttypes-api-openapi.yml
- filename: semaphore-tasks-api-openapi.yml
  format: yaml
  label: Semaphore Tasks API
  slug: semaphore-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-tasks-api-openapi.yml
- filename: semaphore-workflows-api-openapi.yml
  format: yaml
  label: Semaphore Workflows API
  slug: semaphore-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Semaphore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semaphore secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Semaphore
provider_slug: semaphore
scheme_count: 1
schemes:
- description: Token that you get from semaphore [account settings](https://me.semaphoreci.com/account).
  name: authorization
  scheme: bearer
  sources:
  - openapi/semaphore-semaphore-api-openapi.yml
  type: http
slug: semaphore-authentication
source_filename: semaphore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/semaphore-semaphore-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: Token that you get from semaphore [account settings](https://me.semaphoreci.com/account).\n  sources:\n  - openapi/semaphore-semaphore-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/authentication/semaphore-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- Pipelines
- Workflows
- DevOps
- Build Automation
- Software Delivery
- Deployment
- Artifacts
---
