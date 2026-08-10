---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Terminus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminus secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Terminus
provider_slug: terminus
scheme_count: 2
schemes:
- description: Terminus ABM Platform API access is requested through a DemandScience support ticket; the key is issued by a CSM or Onboarding Specialist rather than self-served from a developer console. Anonymous requests to https://api.terminusplatform.com/ return HTTP 401 with the plain-text body "Authentication Invalid" on every path probed.
  in: header
  name: PlatformApiKey
  sources:
  - https://support.demandscience.com/hc/en-us/articles/360051822454-Employee-Automation-API-for-Email-Experiences
  type: apiKey
- description: Web Experiences (terminus.bound360.com) connects to the DemandScience data and advertising audiences using an API key "provided by your CSM or Onboarding Specialist", entered on the Connections page of the web personalization interface.
  in: header
  name: WebExperiencesApiKey
  sources:
  - https://support.demandscience.com/hc/en-us/articles/360045192013-Connecting-Your-Web-Experiences-API-Key
  type: apiKey
slug: terminus-authentication
source_filename: terminus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://support.demandscience.com/hc/en-us\ndocs: https://support.demandscience.com/hc/en-us/articles/360045192013-Connecting-Your-Web-Experiences-API-Key\nnote: >-\n  Derived from the public DemandScience Help Center, not from an OpenAPI — Terminus\n  publishes no machine-readable specification. The API reference lives on a Redocly\n  developer portal at developer.terminus.com where every path 302s to /redocly-login,\n  so the security schemes below are what the public help center documents plus what\n  the live API host returns to an anonymous caller.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  issuance: support-ticket\n  sso: [saml2, oidc, microsoft, google]\nschemes:\n- name: PlatformApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Terminus ABM Platform API access is requested through a DemandScience support\n    ticket; the key is issued by a CSM or Onboarding Specialist rather\
  \ than\n    self-served from a developer console. Anonymous requests to\n    https://api.terminusplatform.com/ return HTTP 401 with the plain-text body\n    \"Authentication Invalid\" on every path probed.\n  sources: [https://support.demandscience.com/hc/en-us/articles/360051822454-Employee-Automation-API-for-Email-Experiences]\n- name: WebExperiencesApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Web Experiences (terminus.bound360.com) connects to the DemandScience data and\n    advertising audiences using an API key \"provided by your CSM or Onboarding\n    Specialist\", entered on the Connections page of the web personalization interface.\n  sources: [https://support.demandscience.com/hc/en-us/articles/360045192013-Connecting-Your-Web-Experiences-API-Key]\nuser_authentication:\n  description: >-\n    Human sign-in to the platform (app.demandscienceplatform.com) supports Microsoft\n    and Google SSO out of the box, plus SAML 2.0 for third-party identity providers\n   \
  \ (both SP-initiated and IdP-initiated), and OpenID Connect as an alternative input\n    set. SAML/OIDC enablement is coordinated by an Account Manager or CSM and may\n    carry additional cost.\n  standards: [saml2, oidc]\n  requires_from_customer:\n    saml2: [idp-sso-url, idp-issuer-uri, x509-certificate, attribute-mappings, saml-metadata-xml]\n    oidc: [issuer, authorization-endpoint, token-endpoint, jwks-uri, userinfo-endpoint]\n  docs: https://support.demandscience.com/hc/en-us/articles/360059215833-Logging-Into-the-DemandScience-Platform-Using-SAML-2-0\nx-evidence:\n- {url: 'https://api.terminusplatform.com/openapi.json', http_status: 401, body: Authentication Invalid, fetched: '2026-08-05'}\n- {url: 'https://api.terminusplatform.com/v1', http_status: 401, body: Authentication Invalid, fetched: '2026-08-05'}\n- {url: 'https://developer.terminus.com/', http_status: 302, redirect: /redocly-login, fetched: '2026-08-05'}\n- {url: 'https://support.demandscience.com/api/v2/help_center/en-us/articles/360045192013.json',\
  \ http_status: 200, fetched: '2026-08-05'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminus/refs/heads/main/authentication/terminus-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Account Based Marketing
- Marketing
- Advertising
- Sales
- B2B
- Analytics
- Email
---
