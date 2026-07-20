---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Insider Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insider secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Insider
provider_slug: insider
scheme_count: 2
schemes:
- description: Generated API key for the account. Sent on every request.
  in: header
  name: RequestToken
  parameter: X-REQUEST-TOKEN
  sources:
  - docs
  type: apiKey
- description: The Insider partner name for the account (auto-populated by the wizard). Paired with X-REQUEST-TOKEN to identify and authorize the caller.
  in: header
  name: PartnerName
  parameter: X-PARTNER-NAME
  sources:
  - docs
  type: apiKey
slug: insider-authentication
source_filename: insider-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://academy.insiderone.com/docs/upsert-user-data-api-integration-wizard-2\ndocs: https://academy.insiderone.com/docs/upsert-user-data-api-integration-wizard-2\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Insider's Unified Customer Database (Upsert User Data API) authenticates with a\n    two-header API-key pair. API credentials are generated per partner/account in\n    the InOne panel via the integration wizard and must be kept confidential;\n    testing is recommended against a UAT account before production.\nschemes:\n- name: RequestToken\n  type: apiKey\n  in: header\n  parameter: X-REQUEST-TOKEN\n  description: Generated API key for the account. Sent on every request.\n  sources: [docs]\n- name: PartnerName\n  type: apiKey\n  in: header\n  parameter: X-PARTNER-NAME\n  description: >-\n    The Insider partner name for the account (auto-populated by the wizard).\n    Paired\
  \ with X-REQUEST-TOKEN to identify and authorize the caller.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/authentication/insider-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Customer Engagement
- Personalization
- Customer Data Platform
- Marketing
- Journey Orchestration
- Omnichannel
- CDP
- Artificial Intelligence
---
