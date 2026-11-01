---
anonymous_access: false
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arda secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arda
provider_slug: arda
scheme_count: 1
schemes:
- description: Pro-plan API key. The pricing-page FAQ states-- "Pro is self-serve. You get an API key and advanced analytics, and your team builds its own integrations and workflows." The Pro tier ($299 /mo per Power User, billed annually) lists "Full API access" and "API access & advanced analytics" as included features; the Team tier lists "Not included-- Full API access". Header name, placement (header vs. query) and format are not published; no public reference documentation, OpenAPI contract or developer portal exists at this provider.
  evidence:
  - quote: Pro is self-serve. You get an API key and advanced analytics, and your team builds its own integrations and workflows.
    url: https://www.arda.cards/pricing
  - quote: Full API access
    url: https://www.arda.cards/pricing
  - quote: Works with the tools you have. Connect Gmail, Sheets, QuickBooks, Shopify, NetSuite, Xero, Airtable, Zapier, and REST APIs.
    url: https://www.arda.cards/features
  gated: true
  name: apiKey
  tier: Pro
  type: apiKey
slug: arda-authentication
source_filename: arda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource:\n- https://www.arda.cards/pricing\n- https://www.arda.cards/features\ndocs: https://www.arda.cards/pricing\nsummary:\n  types:\n  - apiKey\n  note: Arda documents an API key auth model only. No public reference describes\n    the key format, header name, placement, or whether the API is REST / GraphQL\n    / other. Keys are issued to paying Pro-plan customers only; the Team and Free\n    plans are explicitly 'Not included-- Full API access'. No OpenAPI, developer\n    portal, SDK or sandbox is published; details are provided to Pro customers\n    after sign-up.\nschemes:\n- name: apiKey\n  type: apiKey\n  description: 'Pro-plan API key. The pricing-page FAQ states-- \"Pro is self-serve.\n    You get an API key and advanced analytics, and your team builds its own\n    integrations and workflows.\" The Pro tier ($299 /mo per Power User, billed\n    annually) lists \"Full API access\" and \"API access & advanced analytics\" as\n\
  \    included features; the Team tier lists \"Not included-- Full API access\".\n    Header name, placement (header vs. query) and format are not published; no\n    public reference documentation, OpenAPI contract or developer portal exists\n    at this provider.'\n  tier: Pro\n  gated: true\n  evidence:\n  - url: https://www.arda.cards/pricing\n    quote: 'Pro is self-serve. You get an API key and advanced analytics, and your\n      team builds its own integrations and workflows.'\n  - url: https://www.arda.cards/pricing\n    quote: 'Full API access'\n  - url: https://www.arda.cards/features\n    quote: 'Works with the tools you have. Connect Gmail, Sheets, QuickBooks,\n      Shopify, NetSuite, Xero, Airtable, Zapier, and REST APIs.'\n"
source_yaml_url: https://artifacts.apis.io/arda/authentication/arda-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- FinTech
- API
- DigitalAssets
- Trading
---
