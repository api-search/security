---
api_key_in:
- header
- body
api_specs:
- filename: vessel-platform-openapi.yml
  format: yaml
  label: Vessel Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-platform-openapi.yml
- filename: vessel-crm-openapi.yml
  format: yaml
  label: Vessel CRM Unified API
  slug: crm-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-openapi.yml
- filename: vessel-engagement-openapi.yml
  format: yaml
  label: Vessel Sales Engagement Unified API
  slug: engagement-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-openapi.yml
- filename: vessel-chat-openapi.yml
  format: yaml
  label: Vessel Chat Unified API
  slug: chat-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-chat-openapi.yml
- filename: vessel-dialer-openapi.yml
  format: yaml
  label: Vessel Dialer Unified API
  slug: dialer-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-dialer-openapi.yml
- filename: vessel-marketing-automation-openapi.yml
  format: yaml
  label: Vessel Marketing Automation Unified API
  slug: marketing-automation-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-marketing-automation-openapi.yml
- filename: vessel-crm-v1-openapi.yml
  format: yaml
  label: Vessel CRM API (v1, legacy)
  slug: crm-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-v1-openapi.yml
- filename: vessel-engagement-v1-openapi.yml
  format: yaml
  label: Vessel Engagement API (v1, legacy)
  slug: engagement-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-v1-openapi.yml
- filename: vessel-salesforce-actions-openapi.yml
  format: yaml
  label: Vessel Salesforce Actions API
  slug: salesforce-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-salesforce-actions-openapi.yml
- filename: vessel-slack-actions-openapi.yml
  format: yaml
  label: Vessel Slack Actions API
  slug: slack-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-slack-actions-openapi.yml
- filename: vessel-teams-actions-openapi.yml
  format: yaml
  label: Vessel Microsoft Teams Actions API
  slug: teams-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-teams-actions-openapi.yml
- filename: vessel-outreach-actions-openapi.yml
  format: yaml
  label: Vessel Outreach Actions API
  slug: outreach-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-outreach-actions-openapi.yml
- filename: vessel-salesloft-actions-openapi.yml
  format: yaml
  label: Vessel Salesloft Actions API
  slug: salesloft-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-salesloft-actions-openapi.yml
- filename: vessel-apollo-actions-openapi.yml
  format: yaml
  label: Vessel Apollo Actions API
  slug: apollo-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-apollo-actions-openapi.yml
- filename: vessel-aircall-actions-openapi.yml
  format: yaml
  label: Vessel Aircall Actions API
  slug: aircall-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-aircall-actions-openapi.yml
- filename: vessel-dialpad-actions-openapi.yml
  format: yaml
  label: Vessel Dialpad Actions API
  slug: dialpad-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-dialpad-actions-openapi.yml
- filename: vessel-ringcentral-actions-openapi.yml
  format: yaml
  label: Vessel RingCentral Actions API
  slug: ringcentral-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-ringcentral-actions-openapi.yml
- filename: vessel-mailchimp-actions-openapi.yml
  format: yaml
  label: Vessel Mailchimp Actions API
  slug: mailchimp-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-mailchimp-actions-openapi.yml
- filename: vessel-activecampaign-actions-openapi.yml
  format: yaml
  label: Vessel ActiveCampaign Actions API
  slug: activecampaign-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-activecampaign-actions-openapi.yml
- filename: vessel-monday-actions-openapi.yml
  format: yaml
  label: Vessel monday.com Actions API
  slug: monday-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-monday-actions-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vessel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vessel secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vessel
provider_slug: vessel
scheme_count: 4
schemes:
- description: Project API token for the v2 platform, unified and actions APIs on api.vessel.dev. Declared as the documented auth method in the provider's own Mintlify config (`api.auth.name`).
  in: header
  name: VesselAPIToken
  parameter: x-vessel-api-token
  sources:
  - https://github.com/vesselapi/all-api-docs/blob/main/docs/mint.json
  - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/home/webhooks.mdx
  type: apiKey
- description: Project API token for the legacy v1 CRM and Engagement APIs on api.vessel.land. The header name loses the `x-` prefix on the v1 surface — the two generations are not header-compatible.
  in: header
  name: VesselAPIToken
  parameter: vessel-api-token
  sources:
  - openapi/vessel-crm-v1-openapi.yml
  - openapi/vessel-engagement-v1-openapi.yml
  - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/crm/authentication-and-security.mdx
  type: apiKey
- description: Per-connection access token identifying which end-customer account the call acts on. Sent in the request body on POST operations and in the query string on the legacy v1 GET operations. Obtained by exchanging a publicToken (see the Link flow below) and intended to be stored permanently.
  in: body
  name: accessToken
  parameter: accessToken
  sources:
  - openapi/vessel-crm-openapi.yml
  - openapi/vessel-engagement-v1-openapi.yml
  type: apiKey
- description: Short-lived token minted by POST /api/auth/session-token and handed to the browser so the Vessel Link component can start the connect flow without exposing the project API token.
  in: body
  name: sessionToken
  parameter: sessionToken
  sources:
  - openapi/vessel-platform-openapi.yml
  type: apiKey
slug: vessel-authentication
source_filename: vessel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/crm/authentication-and-security.mdx\ndocs:\n  - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/crm/authentication-and-security.mdx\n  - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/home/getting-started.mdx\n  - https://github.com/vesselapi/all-api-docs/blob/main/docs/mint.json\nderived_from:\n  - openapi/vessel-crm-v1-openapi.yml\n  - openapi/vessel-engagement-v1-openapi.yml\n  - openapi/vessel-platform-openapi.yml\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n    - body\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Vessel is a key-auth API with a two-token model. A long-lived project API token authenticates\n    the caller (the \"gated neighborhood\"), and a per-connection accessToken authorizes access to one\n    end-customer's connected account (the \"house\"). There is no OAuth2\
  \ flow for Vessel's own API —\n    OAuth is used only downstream, between Vessel and the end customer's SaaS provider, and Vessel\n    exposes /api/auth/oauth-apps so a customer can bring their own downstream OAuth client.\nschemes:\n  - name: VesselAPIToken\n    type: apiKey\n    in: header\n    parameter: x-vessel-api-token\n    description: >-\n      Project API token for the v2 platform, unified and actions APIs on api.vessel.dev. Declared as\n      the documented auth method in the provider's own Mintlify config (`api.auth.name`).\n    sources:\n      - https://github.com/vesselapi/all-api-docs/blob/main/docs/mint.json\n      - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/home/webhooks.mdx\n  - name: VesselAPIToken\n    type: apiKey\n    in: header\n    parameter: vessel-api-token\n    description: >-\n      Project API token for the legacy v1 CRM and Engagement APIs on api.vessel.land. The header name\n      loses the `x-` prefix on the v1 surface — the two generations\
  \ are not header-compatible.\n    sources:\n      - openapi/vessel-crm-v1-openapi.yml\n      - openapi/vessel-engagement-v1-openapi.yml\n      - https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/crm/authentication-and-security.mdx\n  - name: accessToken\n    type: apiKey\n    in: body\n    parameter: accessToken\n    description: >-\n      Per-connection access token identifying which end-customer account the call acts on. Sent in the\n      request body on POST operations and in the query string on the legacy v1 GET operations. Obtained\n      by exchanging a publicToken (see the Link flow below) and intended to be stored permanently.\n    sources:\n      - openapi/vessel-crm-openapi.yml\n      - openapi/vessel-engagement-v1-openapi.yml\n  - name: sessionToken\n    type: apiKey\n    in: body\n    parameter: sessionToken\n    description: >-\n      Short-lived token minted by POST /api/auth/session-token and handed to the browser so the Vessel\n      Link component can start\
  \ the connect flow without exposing the project API token.\n    sources:\n      - openapi/vessel-platform-openapi.yml\nflows:\n  - name: Vessel Link token exchange\n    description: >-\n      The documented handshake that turns an end user's consent into a durable per-connection credential.\n    steps:\n      - step: 1\n        action: >-\n          Your server calls the link/session token endpoint with the project API token to obtain a\n          linkToken (v1) or sessionToken (v2) — a temporary, client-safe credential.\n        operations:\n          - post-link-token\n          - get-one-session-token\n      - step: 2\n        action: >-\n          The token is passed to the Vessel Link component in the browser. On success the component\n          returns a temporary publicToken to your frontend.\n      - step: 3\n        action: >-\n          Your server exchanges the publicToken for a permanent accessToken.\n        operations:\n          - post-link-exchange\n          - get-one-access-token\n\
  \      - step: 4\n        action: >-\n          Store the accessToken securely. Every subsequent unified/actions call sends the project API\n          token in the header and the accessToken in the body (or query on v1).\ntransport:\n  https_required: true\n  note: >-\n    \"All requests to Vessel are authenticated by an API token and all requests must be made over https.\"\nkey_provisioning:\n  self_serve: false\n  note: >-\n    The docs instruct callers to email support@vessel.dev to request an API token. Each customer is\n    issued two keys — a development key (capped at 5 connections) and a production key.\n  source: https://github.com/vesselapi/all-api-docs/blob/main/docs/pages/home/hidden/error-faq.mdx\nx-observed:\n  checked: '2026-08-13'\n  note: >-\n    Neither api.vessel.dev nor api.vessel.land answered a TLS connection on 2026-08-13, so none of the\n    above could be exercised live. The model is transcribed from the provider's published contracts and\n    documentation, not\
  \ from an observed response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/authentication/vessel-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- CRM
- Chat
- Dialer
- Embedded Integrations
- GTM
- Integrations
- iPaaS
- Marketing Automation
- Sales Engagement
- Unified API
- Webhooks
---
