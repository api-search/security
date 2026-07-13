---
api_key_in:
- header
api_specs:
- filename: dell-servers-idrac-redfish-openapi.yml
  format: yaml
  label: Dell iDRAC Redfish REST API
  slug: dell-servers-idrac-redfish
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-idrac-redfish-openapi.yml
- filename: dell-servers-openmanage-enterprise-openapi.yml
  format: yaml
  label: Dell OpenManage Enterprise API
  slug: dell-servers-openmanage-enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/openapi/dell-servers-openmanage-enterprise-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dell Servers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dell Servers secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dell Servers
provider_slug: dell-servers
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using iDRAC username and password credentials. All API requests require authentication except for the Redfish service root at /redfish/v1.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dell-servers-idrac-redfish-openapi.yml
  type: http
- description: Session-based authentication using a token obtained from the Sessions resource POST operation. The token is passed in the X-Auth-Token header.
  in: header
  name: sessionAuth
  parameter: X-Auth-Token
  sources:
  - openapi/dell-servers-idrac-redfish-openapi.yml
  - openapi/dell-servers-openmanage-enterprise-openapi.yml
  type: apiKey
slug: dell-servers-authentication
source_filename: dell-servers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dell-servers-idrac-redfish-openapi.yml, openapi/dell-servers-openmanage-enterprise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using iDRAC username and password credentials. All\n    API requests require authentication except for the Redfish service root at /redfish/v1.\n  sources:\n  - openapi/dell-servers-idrac-redfish-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: Session-based authentication using a token obtained from the Sessions resource\n    POST operation. The token is passed in the X-Auth-Token header.\n  sources:\n  - openapi/dell-servers-idrac-redfish-openapi.yml\n  - openapi/dell-servers-openmanage-enterprise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dell-servers/refs/heads/main/authentication/dell-servers-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Hardware
- Infrastructure
- Management
- Monitoring
- Servers
---
