---
api_key_in: []
api_specs:
- filename: bodytrace-alerts-api-openapi.yml
  format: yaml
  label: BodyTrace Alerts API
  slug: bodytrace-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-alerts-api-openapi.yml
- filename: bodytrace-data-messages-api-openapi.yml
  format: yaml
  label: BodyTrace Data Messages API
  slug: bodytrace-data-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-data-messages-api-openapi.yml
- filename: bodytrace-devices-api-openapi.yml
  format: yaml
  label: BodyTrace Devices API
  slug: bodytrace-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-devices-api-openapi.yml
- filename: bodytrace-observations-api-openapi.yml
  format: yaml
  label: BodyTrace Observations API
  slug: bodytrace-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-observations-api-openapi.yml
- filename: bodytrace-provisioning-api-openapi.yml
  format: yaml
  label: BodyTrace Provisioning API
  slug: bodytrace-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-provisioning-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bodytrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: BodyTrace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BodyTrace
provider_slug: bodytrace
scheme_count: 1
schemes:
- description: HTTP Basic authentication using the username and password issued by BodyTrace for your account. The same credential model secures the customer-hosted push endpoint (you define the username/password BodyTrace uses when POSTing measurements to you).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bodytrace-openapi.yml
  type: http
slug: bodytrace-authentication
source_filename: bodytrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bodytrace-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the username and password issued by BodyTrace\n    for your account. The same credential model secures the customer-hosted push endpoint (you\n    define the username/password BodyTrace uses when POSTing measurements to you).\n  sources:\n  - openapi/bodytrace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/authentication/bodytrace-authentication.yml
summary_line: http · 1 scheme
tags:
- Remote Patient Monitoring
- RPM
- Cellular
- Medical Devices
- Digital Health
- Blood Pressure
- Connected Devices
- IoT
---
