---
api_key_in: []
api_specs:
- filename: mabl-applications-api-openapi.yml
  format: yaml
  label: Mabl Applications API
  slug: mabl-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-applications-api-openapi.yml
- filename: mabl-credentials-api-openapi.yml
  format: yaml
  label: Mabl Credentials API
  slug: mabl-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-credentials-api-openapi.yml
- filename: mabl-database-connections-api-openapi.yml
  format: yaml
  label: Mabl Database Connections API
  slug: mabl-database-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-database-connections-api-openapi.yml
- filename: mabl-deployment-events-api-openapi.yml
  format: yaml
  label: Mabl Deployment Events API
  slug: mabl-deployment-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-deployment-events-api-openapi.yml
- filename: mabl-environments-api-openapi.yml
  format: yaml
  label: Mabl Environments API
  slug: mabl-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-environments-api-openapi.yml
- filename: mabl-flows-api-openapi.yml
  format: yaml
  label: Mabl Flows API
  slug: mabl-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-flows-api-openapi.yml
- filename: mabl-issues-api-openapi.yml
  format: yaml
  label: Mabl Issues API
  slug: mabl-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-issues-api-openapi.yml
- filename: mabl-test-runs-api-openapi.yml
  format: yaml
  label: Mabl Test Runs API
  slug: mabl-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-test-runs-api-openapi.yml
- filename: mabl-tests-api-openapi.yml
  format: yaml
  label: Mabl Tests API
  slug: mabl-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-tests-api-openapi.yml
- filename: mabl-users-api-openapi.yml
  format: yaml
  label: Mabl Users API
  slug: mabl-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mabl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mabl secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mabl
provider_slug: mabl
scheme_count: 1
schemes:
- description: HTTP Basic with username "key" and a mabl API key as the password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mabl-openapi.yml
  type: http
slug: mabl-authentication
source_filename: mabl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mabl-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with username \"key\" and a mabl API key as the password.\n  sources:\n  - openapi/mabl-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/authentication/mabl-authentication.yml
summary_line: http · 1 scheme
tags:
- Test Automation
- QA
- DevOps
- AI Testing
- Platform
---
