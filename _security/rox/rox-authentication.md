---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rox declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Rox
provider_slug: rox
scheme_count: 0
schemes: []
slug: rox-authentication
source_filename: rox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.rox.com/development/engineering/docs/rox-enterprise-integrations/enterprise-sso-via-auth0.md\napi_authentication_published: false\npointer_emitted: false\npointer_note: >-\n  No `Authentication` pointer is wired in apis.yml. Rox publishes no public REST\n  API, so there is no API authentication scheme to document; what follows is the\n  END-USER and INTEGRATION authentication posture, recorded for completeness.\n  Emitting an Authentication pointer here would credit Rox with API auth\n  documentation it does not publish — the same false-credit failure mode as a\n  well-known pointer over a 404 probe.\nsurfaces:\n- surface: application-signin\n  host: run.rox.com\n  broker: Auth0\n  broker_evidence: >-\n    Rox's published subprocessor list names \"Auth0, Inc. — Authentication\", and\n    the enterprise SSO documentation is titled \"Enterprise SSO via Auth0\".\n  methods:\n  - id: email-password\n    docs: https://docs.rox.com/development/product/accessing-rox/login-with-email-and-password\n\
  \  - id: google\n    docs: https://docs.rox.com/development/product/accessing-rox/login-with-google\n  - id: microsoft\n    description: '\"Continue with Microsoft\" via an Auth0 Enterprise connection to Microsoft Entra ID.'\n    docs: https://docs.rox.com/development/engineering/docs/rox-enterprise-integrations/outlook-sso-via-auth0\n  - id: enterprise-sso\n    protocols:\n    - SAML\n    - OpenID Connect\n    identity_providers_named:\n    - Okta\n    - Microsoft Entra ID\n    self_serve: true\n    self_serve_note: >-\n      \"Enterprise SSO Self Serve\" shipped 2026-07-01 — admins configure SSO from\n      Rox admin settings with no Rox intervention required.\n    docs: https://docs.rox.com/development/engineering/docs/rox-enterprise-integrations/enterprise-sso-via-auth0\n- surface: workflow-webhook\n  host: webhooks.backend.rox.com\n  scheme: none\n  description: >-\n    The inbound Agent Workflow webhook endpoint documents no authentication. The\n    per-workflow slug embedded in\
  \ the URL is the only secret; no signature\n    header, timestamp or verification handshake is published.\n  reference: asyncapi/rox-webhooks.yml\n- surface: outbound-integrations\n  description: >-\n    Rox authenticates OUTWARD to third-party systems via OAuth-style org-wide\n    authorization grants an IT administrator approves — Microsoft Graph, Google\n    Workspace, Zoom Cloud, Microsoft Teams, Slack, Salesforce — plus warehouse\n    credentials for Snowflake, Databricks and BigQuery. These are Rox consuming\n    other providers' APIs, not Rox exposing one.\n  docs: https://docs.rox.com/development/engineering/docs/rox-enterprise-integrations\n- surface: customer-supplied-provider-keys\n  description: >-\n    Enterprise customers may store their own third-party enrichment API keys at\n    the organization level (all supported providers; self-serve accounts are\n    limited to HG Insights). Keys are held by Rox and used on the customer's\n    behalf — again inbound-to-Rox key custody,\
  \ not a Rox API credential.\n  docs: https://docs.rox.com/development/product/people/adding-provider-keys\nwell_known:\n  openid_configuration_served: false\n  oauth_authorization_server_served: false\n  note: >-\n    No OIDC/OAuth discovery metadata is served on any rox.com host; the Auth0\n    tenant is not published. See well-known/rox-well-known.yml for the probe.\nevidence:\n- url: https://docs.rox.com/development/engineering/docs/rox-enterprise-integrations/enterprise-sso-via-auth0.md\n  status: 200\n  fetched: '2026-08-13'\n- url: https://docs.rox.com/development/product/people/adding-provider-keys.md\n  status: 200\n  fetched: '2026-08-13'\n- url: https://run.rox.com/.well-known/openid-configuration\n  status: 404\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rox/refs/heads/main/authentication/rox-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Sales
- Revenue Operations
- Go-to-Market
- CRM
- Sales Intelligence
- Enterprise
- Revenue Intelligence
---
