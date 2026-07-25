---
api_key_in: []
api_specs:
- filename: rhel-advisories-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Advisories API
  slug: rhel-advisories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-advisories-api-openapi.yml
- filename: rhel-cves-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux CVEs API
  slug: rhel-cves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-cves-api-openapi.yml
- filename: rhel-oval-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux OVAL API
  slug: rhel-oval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-oval-api-openapi.yml
- filename: rhel-subscriptions-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Subscriptions API
  slug: rhel-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-subscriptions-api-openapi.yml
- filename: rhel-systems-api-openapi.yml
  format: yaml
  label: Red Hat Enterprise Linux Systems API
  slug: rhel-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-systems-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Rhel Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Red Hat Enterprise Linux secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/rhel-subscription-management-openapi.yml
  type: oauth2
slug: rhel-authentication
source_filename: rhel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rhel-subscription-management-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token\n    scopes: 0\n  sources:\n  - openapi/rhel-subscription-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/authentication/rhel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
---
