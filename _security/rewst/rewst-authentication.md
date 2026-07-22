---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rewst Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rewst secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rewst
provider_slug: rewst
scheme_count: 2
schemes:
- description: Shared secret configured per webhook trigger. When set, callers must send the matching value in the x-rewst-secret header or receive HTTP 401. Secrets can be stored in Rewst Organization Variables.
  in: header
  name: WebhookSecret
  parameter_name: x-rewst-secret
  required: false
  source: https://docs.rewst.help/documentation/automations/intro-to-triggers/use-cases-and-examples/using-webhook-triggers.md
  type: apiKey
- description: Interactive user sign-in to the Rewst application is handled by Auth0-hosted OpenID Connect. This governs human login to app.rewst.io, not webhook/API calls.
  in: browser
  name: Auth0OIDC
  required: true
  source: https://github.com/RewstApp/nextjs-auth0
  type: openIdConnect
slug: rewst-authentication
source_filename: rewst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rewst.help/documentation/app-builder/authentication.md\ndocs: https://docs.rewst.help/documentation/automations/intro-to-triggers/use-cases-and-examples/using-webhook-triggers.md\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    Rewst has no broadly published public REST/OpenAPI reference. Its documented\n    programmatic surface is the inbound webhook trigger, authenticated with an\n    optional shared secret sent in the x-rewst-secret header. The Rewst web app\n    (app.rewst.io) itself authenticates users via Auth0-hosted OIDC (see the\n    RewstApp/nextjs-auth0 repository), but that is the interactive login flow,\n    not a documented machine-to-machine API auth scheme.\nschemes:\n- name: WebhookSecret\n  type: apiKey\n  in: header\n  parameter_name: x-rewst-secret\n  required: false\n  description: >-\n    Shared secret configured per webhook trigger. When set, callers must send the\n\
  \    matching value in the x-rewst-secret header or receive HTTP 401. Secrets can be\n    stored in Rewst Organization Variables.\n  source: https://docs.rewst.help/documentation/automations/intro-to-triggers/use-cases-and-examples/using-webhook-triggers.md\n- name: Auth0OIDC\n  type: openIdConnect\n  in: browser\n  required: true\n  description: >-\n    Interactive user sign-in to the Rewst application is handled by Auth0-hosted\n    OpenID Connect. This governs human login to app.rewst.io, not webhook/API calls.\n  source: https://github.com/RewstApp/nextjs-auth0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rewst/refs/heads/main/authentication/rewst-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Devops
- Automation
- iPaaS
- RPA
- Workflow Automation
- MSP
- Integration
- Webhooks
---
