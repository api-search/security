---
api_key_in: []
api_specs:
- filename: cisco-collaboration-hybrid-solutions-devices-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Devices API
  slug: cisco-collaboration-hybrid-solutions-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-devices-api-openapi.yml
- filename: cisco-collaboration-hybrid-solutions-memberships-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Memberships API
  slug: cisco-collaboration-hybrid-solutions-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-memberships-api-openapi.yml
- filename: cisco-collaboration-hybrid-solutions-messages-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Messages API
  slug: cisco-collaboration-hybrid-solutions-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-messages-api-openapi.yml
- filename: cisco-collaboration-hybrid-solutions-rooms-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Rooms API
  slug: cisco-collaboration-hybrid-solutions-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-rooms-api-openapi.yml
- filename: cisco-collaboration-hybrid-solutions-teams-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Teams API
  slug: cisco-collaboration-hybrid-solutions-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-teams-api-openapi.yml
- filename: cisco-collaboration-hybrid-solutions-webhooks-api-openapi.yml
  format: yaml
  label: Cisco Collaboration Hybrid Solutions Webhooks API
  slug: cisco-collaboration-hybrid-solutions-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/openapi/cisco-collaboration-hybrid-solutions-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Collaboration Hybrid Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Collaboration Hybrid Solutions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Collaboration Hybrid Solutions
provider_slug: cisco-collaboration-hybrid-solutions
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-collaboration-hybrid-solutions-openapi.yml
  type: http
slug: cisco-collaboration-hybrid-solutions-authentication
source_filename: cisco-collaboration-hybrid-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-collaboration-hybrid-solutions-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/cisco-collaboration-hybrid-solutions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-collaboration-hybrid-solutions/refs/heads/main/authentication/cisco-collaboration-hybrid-solutions-authentication.yml
summary_line: http · 1 scheme
tags:
- Calling
- Collaboration
- Hybrid Cloud
- Meetings
- Messaging
- Unified Communications
- Webex
---
