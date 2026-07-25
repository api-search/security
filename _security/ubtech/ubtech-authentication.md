---
api_key_in: []
api_specs:
- filename: ubtech-subscriptions-api-openapi.yml
  format: yaml
  label: UBTech subscriptions API
  slug: ubtech-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubtech/refs/heads/main/openapi/ubtech-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Ubtech Authentication
name_suffix: Authentication
oauth_flows: []
overview: UBTech declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: UBTech
provider_slug: ubtech
scheme_count: 0
schemes: []
slug: ubtech-authentication
source_filename: ubtech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/ubtech-yanshee-openadk-openapi-original.yml\nsummary:\n  types: []\n  notes: >-\n    The published Yanshee Open ADK Swagger 2.0 spec declares no\n    securityDefinitions (an oauth2/apiKey example block exists but is\n    commented out). The Yanshee robot API is a device-local HTTP API on the\n    LAN (http://<robot-ip>:9090/v1) with no documented authentication; the\n    subscription callback surface (127.0.0.1:10101) is likewise\n    unauthenticated. Cloud account services (account.ubtrobot.com) exist for\n    UBTech apps but publish no developer-facing auth documentation.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubtech/refs/heads/main/authentication/ubtech-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Robotics
- Humanoid Robots
- Education Technology
- Artificial Intelligence
- Consumer Electronics
- Service Robots
---
