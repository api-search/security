---
api_key_in: []
api_specs:
- filename: teamcity-agent-pools-api-openapi.yml
  format: yaml
  label: TeamCity Agent Pools API
  slug: teamcity-agent-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-agent-pools-api-openapi.yml
- filename: teamcity-agents-api-openapi.yml
  format: yaml
  label: TeamCity Agents API
  slug: teamcity-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-agents-api-openapi.yml
- filename: teamcity-audit-api-openapi.yml
  format: yaml
  label: TeamCity Audit API
  slug: teamcity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-audit-api-openapi.yml
- filename: teamcity-build-configurations-api-openapi.yml
  format: yaml
  label: TeamCity Build Configurations API
  slug: teamcity-build-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-build-configurations-api-openapi.yml
- filename: teamcity-build-queue-api-openapi.yml
  format: yaml
  label: TeamCity Build Queue API
  slug: teamcity-build-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-build-queue-api-openapi.yml
- filename: teamcity-builds-api-openapi.yml
  format: yaml
  label: TeamCity Builds API
  slug: teamcity-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-builds-api-openapi.yml
- filename: teamcity-changes-api-openapi.yml
  format: yaml
  label: TeamCity Changes API
  slug: teamcity-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-changes-api-openapi.yml
- filename: teamcity-cloud-api-openapi.yml
  format: yaml
  label: TeamCity Cloud API
  slug: teamcity-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-cloud-api-openapi.yml
- filename: teamcity-investigations-api-openapi.yml
  format: yaml
  label: TeamCity Investigations API
  slug: teamcity-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-investigations-api-openapi.yml
- filename: teamcity-mutes-api-openapi.yml
  format: yaml
  label: TeamCity Mutes API
  slug: teamcity-mutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-mutes-api-openapi.yml
- filename: teamcity-problems-api-openapi.yml
  format: yaml
  label: TeamCity Problems API
  slug: teamcity-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-problems-api-openapi.yml
- filename: teamcity-projects-api-openapi.yml
  format: yaml
  label: TeamCity Projects API
  slug: teamcity-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-projects-api-openapi.yml
- filename: teamcity-server-api-openapi.yml
  format: yaml
  label: TeamCity Server API
  slug: teamcity-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-server-api-openapi.yml
- filename: teamcity-tests-api-openapi.yml
  format: yaml
  label: TeamCity Tests API
  slug: teamcity-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-tests-api-openapi.yml
- filename: teamcity-user-groups-api-openapi.yml
  format: yaml
  label: TeamCity User Groups API
  slug: teamcity-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-user-groups-api-openapi.yml
- filename: teamcity-users-api-openapi.yml
  format: yaml
  label: TeamCity Users API
  slug: teamcity-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-users-api-openapi.yml
- filename: teamcity-vcs-roots-api-openapi.yml
  format: yaml
  label: TeamCity VCS Roots API
  slug: teamcity-vcs-roots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/openapi/teamcity-vcs-roots-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teamcity Authentication
name_suffix: Authentication
oauth_flows: []
overview: TeamCity secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TeamCity
provider_slug: teamcity
scheme_count: 2
schemes:
- description: Bearer token authentication using access tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teamcity-rest-api.yml
  type: http
- description: HTTP Basic authentication with username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/teamcity-rest-api.yml
  type: http
slug: teamcity-authentication
source_filename: teamcity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teamcity-rest-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using access tokens\n  sources:\n  - openapi/teamcity-rest-api.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with username and password\n  sources:\n  - openapi/teamcity-rest-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamcity/refs/heads/main/authentication/teamcity-authentication.yml
summary_line: http · 2 schemes
tags:
- Build Automation
- CI/CD
- Continuous Integration
- Deployment
- DevOps
- Testing
---
