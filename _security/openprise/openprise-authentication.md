---
api_key_in:
- header
auth_types:
- apiKey
- saml2
description: Authentication profile for the Openprise API Factory surface and for the Openprise Cloud platform itself. Derived from the provider's own Help Center rather than from an OpenAPI document — Openprise publishes no machine-readable specification, because every API Factory endpoint is generated per tenant from a customer-configured Job or Bot and its contract is shown inside the application ("View API Docs").
kind: authentication
layout: security
method: searched
name: Openprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openprise secures its APIs with apiKey and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Openprise
provider_slug: openprise
scheme_count: 3
schemes:
- applies_to: API Factory generated REST endpoints (API Jobs and API Bots)
  header_name: null
  header_name_note: The exact header name is not published. The Help Center shows it only as a screenshot of the Custom Headers panel ("an example of custom headers needed for Openprise's API Factory") on the Call Simple REST API task page, and the endpoint contract itself is revealed in the in-app "View API Docs" popup. Recorded as null rather than guessed.
  in: header
  name: API Factory API key
  provisioning: Per user, inside the tenant. The user clicks their username, opens the My Account page, and generates a key on the API Key tab. API Factory must first be switched on for the whole tenant by an Openprise System Administrator under Administration → Settings → Features, and it is a separately licensed feature.
  source: https://helpcenter.openprisetech.com/hc/en-us/articles/24107925788180-API-Factory-Overview-and-Use-Guide
  surface: inbound
  type: apiKey
- applies_to: Third-party services Openprise calls through the Simple REST API (Webhook) data service and task template.
  in: header
  name: Data Service API key
  provisioning: Stored as an Account on a Data Service under Data → Data Services. The key is then exposed to the job as a "Data Service api key" attribute that can be interpolated into the URL, Custom Headers, or Request Body of the Call Simple REST API task.
  source: https://helpcenter.openprisetech.com/hc/en-us/articles/27778785661588-Simple-Rest-API-Webhook-Data-Service
  surface: outbound
  type: apiKey
- applies_to: Openprise Cloud web application (https://www.openprisecloud.com)
  identity_providers:
  - Okta
  - OneLogin
  - Oracle Access Manager
  - Ping Federate
  name: SAML 2.0 single sign-on
  note: Configured under Administration → Security Settings → SSO Integration. Ping SSO support was added in the May 30, 2026 release. Password policy (minimum length, composition rules, and a default 5-month rotation) is configured on the same page.
  source: https://helpcenter.openprisetech.com/hc/en-us/articles/24107864003732-Single-Sign-On-SSO-Configuration
  surface: platform-login
  type: saml2
slug: openprise-authentication
source_filename: openprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://helpcenter.openprisetech.com/hc/en-us/articles/24107925788180-API-Factory-Overview-and-Use-Guide\ndocs: https://helpcenter.openprisetech.com/hc/en-us/articles/24107925788180-API-Factory-Overview-and-Use-Guide\nprovider: Openprise\nproviderId: openprise\ndescription: >-\n  Authentication profile for the Openprise API Factory surface and for the Openprise\n  Cloud platform itself. Derived from the provider's own Help Center rather than from\n  an OpenAPI document — Openprise publishes no machine-readable specification, because\n  every API Factory endpoint is generated per tenant from a customer-configured Job or\n  Bot and its contract is shown inside the application (\"View API Docs\").\nsummary:\n  types:\n    - apiKey\n    - saml2\n  api_key_in:\n    - header\n  oauth2_flows: []\n  oauth2_supported: false\n  note: >-\n    Openprise's own Help Center states plainly, on the Call Simple REST API (Webhook)\n    task template\
  \ page, \"At this time, Openprise does not support authentication using\n    OAuth to the API service. We only support API key authentication.\" That sentence is\n    about Openprise calling OUT to a third-party service, and it is the clearest\n    published statement of the platform's auth posture. No OAuth 2.0 or OpenID Connect\n    surface was found on either direction of the integration.\nschemes:\n  - name: API Factory API key\n    type: apiKey\n    in: header\n    surface: inbound\n    applies_to: API Factory generated REST endpoints (API Jobs and API Bots)\n    provisioning: >-\n      Per user, inside the tenant. The user clicks their username, opens the My Account\n      page, and generates a key on the API Key tab. API Factory must first be switched\n      on for the whole tenant by an Openprise System Administrator under Administration\n      → Settings → Features, and it is a separately licensed feature.\n    header_name: null\n    header_name_note: >-\n      The exact header\
  \ name is not published. The Help Center shows it only as a\n      screenshot of the Custom Headers panel (\"an example of custom headers needed for\n      Openprise's API Factory\") on the Call Simple REST API task page, and the endpoint\n      contract itself is revealed in the in-app \"View API Docs\" popup. Recorded as null\n      rather than guessed.\n    source: https://helpcenter.openprisetech.com/hc/en-us/articles/24107925788180-API-Factory-Overview-and-Use-Guide\n  - name: Data Service API key\n    type: apiKey\n    in: header\n    surface: outbound\n    applies_to: >-\n      Third-party services Openprise calls through the Simple REST API (Webhook) data\n      service and task template.\n    provisioning: >-\n      Stored as an Account on a Data Service under Data → Data Services. The key is then\n      exposed to the job as a \"Data Service api key\" attribute that can be interpolated\n      into the URL, Custom Headers, or Request Body of the Call Simple REST API task.\n  \
  \  source: https://helpcenter.openprisetech.com/hc/en-us/articles/27778785661588-Simple-Rest-API-Webhook-Data-Service\n  - name: SAML 2.0 single sign-on\n    type: saml2\n    surface: platform-login\n    applies_to: Openprise Cloud web application (https://www.openprisecloud.com)\n    identity_providers:\n      - Okta\n      - OneLogin\n      - Oracle Access Manager\n      - Ping Federate\n    note: >-\n      Configured under Administration → Security Settings → SSO Integration. Ping SSO\n      support was added in the May 30, 2026 release. Password policy (minimum length,\n      composition rules, and a default 5-month rotation) is configured on the same page.\n    source: https://helpcenter.openprisetech.com/hc/en-us/articles/24107864003732-Single-Sign-On-SSO-Configuration\ncredential_governance:\n  - Credentials are shared to Openprise groups rather than individuals; group-level read\n    and edit permissions are set on each connection under Security Settings → Credentials.\n  - Stored\
  \ third-party credentials are encrypted with a 256-bit key, per the published\n    security policy.\n  - Role-based permissions and delegated administration are listed on both published\n    plan tiers.\nevidence:\n  - url: https://helpcenter.openprisetech.com/hc/en-us/articles/24107925788180-API-Factory-Overview-and-Use-Guide\n    http_status: 200\n    via: Zendesk Help Center API (/api/v2/help_center/en-us/articles/24107925788180.json)\n  - url: https://helpcenter.openprisetech.com/hc/en-us/articles/27776528482324-Call-Simple-REST-API-Webhook\n    http_status: 200\n    via: Zendesk Help Center API\n  - url: https://helpcenter.openprisetech.com/hc/en-us/articles/24107901992084-Security-Settings\n    http_status: 200\n    via: Zendesk Help Center API\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openprise/refs/heads/main/authentication/openprise-authentication.yml
summary_line: apiKey/saml2 · 3 schemes
tags:
- Data Automation
- Data Quality
- Data Orchestration
- AI Orchestration
- Data Enrichment
- Deduplication
- Marketing Operations
- Revenue Operations
- Sales Operations
- Go-To-Market
---
