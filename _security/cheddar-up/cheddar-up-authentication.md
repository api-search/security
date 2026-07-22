---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cheddar Up Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cheddar Up secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cheddar Up
provider_slug: cheddar-up
scheme_count: 2
schemes:
- availability: Team plan
  description: API key credential provisioned to Team-plan accounts to authenticate programmatic integrations. Exact transport (header vs query) is not published on an accessible page and is intentionally left unspecified.
  evidence: https://www.cheddarup.com/integrations/
  name: apiKey
  type: apiKey
- applies_to: JavaScript SDK Checkout component
  description: Guest-facing checkout component requires no authentication token.
  evidence: https://docs.cheddarup.com/javascript-sdk/component-use/checkout
  name: none
  type: none
slug: cheddar-up-authentication
source_filename: cheddar-up-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource:\n- https://www.cheddarup.com/integrations/\n- https://docs.cheddarup.com/javascript-sdk/component-use/checkout\ndocs: https://docs.cheddarup.com/\nsummary:\n  types:\n  - apiKey\n  notes: >-\n    Cheddar Up issues an API key to accounts on the Team plan for REST/webhook\n    integrations. The public JavaScript SDK Checkout component requires no auth\n    token because it is guest/payer-facing against an existing collection.\nschemes:\n- name: apiKey\n  type: apiKey\n  availability: Team plan\n  evidence: https://www.cheddarup.com/integrations/\n  description: >-\n    API key credential provisioned to Team-plan accounts to authenticate\n    programmatic integrations. Exact transport (header vs query) is not\n    published on an accessible page and is intentionally left unspecified.\n- name: none\n  type: none\n  applies_to: JavaScript SDK Checkout component\n  evidence: https://docs.cheddarup.com/javascript-sdk/component-use/checkout\n\
  \  description: Guest-facing checkout component requires no authentication token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheddar-up/refs/heads/main/authentication/cheddar-up-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Payments
- Group Payments
- Fundraising
- Nonprofits
- Schools
- Forms
- Fintech
- Payment Collection
---
