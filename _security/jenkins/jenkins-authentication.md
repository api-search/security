---
api_key_in: []
api_specs:
- filename: jenkins-openapi.yml
  format: yaml
  label: Jenkins Remote Access API
  slug: jenkins-remote-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/openapi/jenkins-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Jenkins Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jenkins secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jenkins
provider_slug: jenkins
scheme_count: 1
schemes:
- description: HTTP Basic auth using a Jenkins username and an API token (not the account password). API tokens are generated per-user under the user's Security configuration and can be revoked independently.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/jenkins-openapi.yml
  type: http
slug: jenkins-authentication
source_filename: jenkins-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/jenkins-openapi.yml\ndocs: https://www.jenkins.io/doc/book/system-administration/authenticating-scripted-clients/\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  credential: username + API token\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic auth using a Jenkins username and an API token (not the account\n    password). API tokens are generated per-user under the user's Security\n    configuration and can be revoked independently.\n  sources:\n  - openapi/jenkins-openapi.yml\ncsrf:\n  required_for: state-changing POST requests (e.g. triggering builds)\n  mechanism: Jenkins-Crumb CSRF token\n  crumb_endpoint: /crumbIssuer/api/json\nnotes: >-\n  SSH public-key auth is also supported for the Jenkins CLI. See\n  cli/jenkins-cli.yml. Some deployments front Jenkins with a reverse-proxy or\n  SSO, but the native scripted-client mechanism is Basic auth with an API\
  \ token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenkins/refs/heads/main/authentication/jenkins-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- Build Server
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Open Source
- Remote Access API
---
