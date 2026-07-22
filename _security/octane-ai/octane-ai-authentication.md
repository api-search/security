---
api_key_in:
- account-settings
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Octane Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octane AI secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Octane AI
provider_slug: octane-ai
scheme_count: 3
schemes:
- description: Per-account API key surfaced in the Octane AI dashboard account settings, used to authenticate integrations and automation platform connections.
  in: account-settings
  name: account_api_key
  sources:
  - https://help.octaneai.com/en/collections/3929090-integrations
  type: apiKey
- description: Per-account webhook signing secret used to verify the authenticity of outbound webhook payloads delivered to connected integration partners.
  in: account-settings
  name: webhook_secret
  sources:
  - https://help.octaneai.com/en/collections/3929090-integrations
  type: apiKey
- description: App installation and store authorization is performed through the Shopify app OAuth flow when a merchant installs Octane AI from the Shopify App Store.
  name: shopify_oauth
  sources:
  - https://octaneai.com/integrations
  type: oauth2
slug: octane-ai-authentication
source_filename: octane-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://help.octaneai.com/en/collections/3929090-integrations\ndocs: https://help.octaneai.com/en/collections/3929090-integrations\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - account-settings\n  oauth2_flows: []\n  notes: >-\n    Octane AI is a Shopify quiz / product-recommendation application. It does not\n    publish a public REST API or OpenAPI. Integration authentication is handled\n    through a per-account API key plus a webhook secret (documented in the help\n    center as \"How do I find my account's API key & webhook secret?\"). These\n    credentials are used by outbound integrations (Zapier, Alloy, marketing\n    platforms) and to verify inbound webhook signatures. The app itself is\n    installed and authorized via Shopify OAuth as an embedded Shopify app.\nschemes:\n- name: account_api_key\n  type: apiKey\n  in: account-settings\n  description: >-\n    Per-account API key surfaced in the Octane AI dashboard\
  \ account settings,\n    used to authenticate integrations and automation platform connections.\n  sources:\n  - https://help.octaneai.com/en/collections/3929090-integrations\n- name: webhook_secret\n  type: apiKey\n  in: account-settings\n  description: >-\n    Per-account webhook signing secret used to verify the authenticity of\n    outbound webhook payloads delivered to connected integration partners.\n  sources:\n  - https://help.octaneai.com/en/collections/3929090-integrations\n- name: shopify_oauth\n  type: oauth2\n  description: >-\n    App installation and store authorization is performed through the Shopify\n    app OAuth flow when a merchant installs Octane AI from the Shopify App Store.\n  sources:\n  - https://octaneai.com/integrations\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octane-ai/refs/heads/main/authentication/octane-ai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Shopify
- E-Commerce
- Product Recommendations
- Quizzes
- Personalization
- Zero-Party Data
- Marketing
- Conversion Optimization
- Artificial Intelligence
---
