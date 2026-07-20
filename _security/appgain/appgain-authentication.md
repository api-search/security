---
api_key_in:
- header
api_specs:
- filename: T17KeScV
  format: yaml
  label: Appgain OmniChannel Messaging API
  slug: appgain-omnichannel-messaging-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/4679101/T17KeScV?version=latest
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appgain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appgain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appgain
provider_slug: appgain
scheme_count: 1
schemes:
- description: Application API key issued per project. Passed as the `appApiKey` request header on every REST call (verified across the public Postman collection).
  in: header
  name: appApiKey
  parameter_name: appApiKey
  sources:
  - postman/T17KeScV
  type: apiKey
slug: appgain-authentication
source_filename: appgain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://documenter.getpostman.com/view/4679101/T17KeScV + https://docs.appgain.io/overview/AppBoostIntegration/\ndocs: https://docs.appgain.io/complete-knowledge-base/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: Appgain's REST API uses a per-application API key sent in an HTTP header, with\n    the tenant/project scoped by a projectId in the request path. There is no OAuth2 or\n    OIDC flow on the messaging API; the API key and project ID are issued from the\n    dashboard under Project Settings -> API and SDK Keys.\nschemes:\n- name: appApiKey\n  type: apiKey\n  in: header\n  parameter_name: appApiKey\n  description: Application API key issued per project. Passed as the `appApiKey` request\n    header on every REST call (verified across the public Postman collection).\n  sources: [postman/T17KeScV]\npath_scoping:\n  parameter: projectId\n  location: path\n  example: https://api.appgain.io/apps/{projectId}/smartlinks\n\
  credentials_source: Project Settings -> API and SDK Keys (Appgain dashboard)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appgain/refs/heads/main/authentication/appgain-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mobile Marketing
- Marketing Automation
- Omnichannel Messaging
- Push Notifications
- SMS
- Email
- WhatsApp
- Customer Data Platform
- Deep Linking
- Customer Engagement
---
