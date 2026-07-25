---
api_key_in: []
api_specs:
- filename: apache-james-domains-api-openapi.yml
  format: yaml
  label: Apache James Domains API
  slug: apache-james-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-domains-api-openapi.yml
- filename: apache-james-healthcheck-api-openapi.yml
  format: yaml
  label: Apache James HealthCheck API
  slug: apache-james-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-healthcheck-api-openapi.yml
- filename: apache-james-mailboxes-api-openapi.yml
  format: yaml
  label: Apache James Mailboxes API
  slug: apache-james-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailboxes-api-openapi.yml
- filename: apache-james-mailqueues-api-openapi.yml
  format: yaml
  label: Apache James MailQueues API
  slug: apache-james-mailqueues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailqueues-api-openapi.yml
- filename: apache-james-mailrepositories-api-openapi.yml
  format: yaml
  label: Apache James MailRepositories API
  slug: apache-james-mailrepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-mailrepositories-api-openapi.yml
- filename: apache-james-quotas-api-openapi.yml
  format: yaml
  label: Apache James Quotas API
  slug: apache-james-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-quotas-api-openapi.yml
- filename: apache-james-tasks-api-openapi.yml
  format: yaml
  label: Apache James Tasks API
  slug: apache-james-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-tasks-api-openapi.yml
- filename: apache-james-users-api-openapi.yml
  format: yaml
  label: Apache James Users API
  slug: apache-james-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/openapi/apache-james-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache James Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache James secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache James
provider_slug: apache-james
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/apache-james-webadmin-rest-api.yaml
  type: http
slug: apache-james-authentication
source_filename: apache-james-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-james-webadmin-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/apache-james-webadmin-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/authentication/apache-james-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
---
