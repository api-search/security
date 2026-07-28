---
api_key_in: []
auth_types:
- none
- oidc-human-login
description: ''
kind: authentication
layout: security
method: probed
name: Saskpower Authentication
name_suffix: Authentication
oauth_flows: []
overview: SaskPower secures its APIs with none and oidc-human-login across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SaskPower
provider_slug: saskpower
scheme_count: 4
schemes:
- applies_to:
  - saskpower:saskpower-power-use-dashboard-data
  - saskpower:saskpower-planned-outages-rss-feed
  - saskpower:saskpower-live-outage-json-feed
  - saskpower:saskpower-outage-map-kml-feed
  - saskpower:saskpower-smart-meter-installation-map-kml-feed
  cors: 'No Access-Control-Allow-Origin header is returned, tested with an explicit Origin: https://example.com. Browser-side third-party use is therefore blocked by the same-origin policy; these feeds are reachable server-side only.'
  detail: 'Anonymous HTTPS GET. Verified 2026-07-27 against all five endpoints with no Authorization header, no cookie, no API key and no Referer: every one returned HTTP 200 with its full payload. No key, no signup, no quota and no published rate limit. The endpoints do set a Sitecore SP_CACHE_KEY session cookie on the response (path=/, secure, HttpOnly, SameSite=None) but do not require it on the request.'
  name: none
  type: none
- applies_to: MySaskPower customer portal (not an API)
  delegated_access: false
  detail: A human browser login, not an authorization surface. There is no client registration, no consent screen offered to a third party, no scope vocabulary, no token endpoint published, and no documented way for an application to be authorized to read another person's data. A customer can reach an in-portal "Download Data" report page (/Profile/My-Dashboard/My-Reports/Download-Data) but no export format is advertised anywhere on the public site and the page itself is behind the login, so no format is recorded here.
  evidence: https://www.saskpower.com/profile/my-dashboard and https://www.saskpower.com/Profile/My-Dashboard/My-Reports/Download-Data both return a 519-byte auto-submitting HTML form POSTing to /identity/externallogin?authenticationType=SaskPower.Azure.B2C with a ReturnUrl back to the requested page. Confirmed 2026-07-27.
  identity_provider: Azure AD B2C, fronted by Sitecore Identity
  name: SaskPower.Azure.B2C
  session_endpoints_observed:
  - /api/sitecore/B2CAuthentication/ExtendLoginCookie
  - /api/sitecore/B2CAuthentication/Logout
  type: openIdConnect
- applies_to: partner.saskpower.com
  detail: 302s to login.microsoftonline.com, tenant dbe9bd7b-4b3a-44b3-b358-e61ff34d58b2, response_type=code id_token, scope=openid profile. Corporate partner SSO for contractors and vendors, not a developer portal and not an API gate.
  name: Microsoft Entra ID (partner portal)
  type: openIdConnect
- applies_to: api.saskpower.com
  detail: 'The gateway is live — CNAME saskpower1.api.mashery.com — but no service is mapped to any public path: every path probed returns HTTP 596 with x-mashery-error-code ERR_596_SERVICE_NOT_FOUND from Server: Mashery Proxy. Mashery''s normal auth model is an api_key/sig query pair, but nothing is exposed to confirm which scheme any real service behind it uses, so the type is recorded as unknown rather than guessed. The developer portal that would have issued keys, api-info.saskpower.com, is NXDOMAIN.'
  name: TIBCO Cloud API Management (Mashery) gateway
  type: unknown
slug: saskpower-authentication
source_filename: saskpower-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live HTTP probes of every SaskPower host and endpoint, 2026-07-27\nnote: >-\n  SaskPower publishes no OpenAPI, so there are no securitySchemes to derive from.\n  This profile is built from what the endpoints and hosts actually do when probed.\n  The estate splits cleanly in two: everything a developer can reach is\n  unauthenticated, and everything authenticated is a human web login with no\n  delegated-authorization path for a third party.\nsummary:\n  types: [none, oidc-human-login]\n  api_key_in: []\n  oauth2_flows: []\n  developer_credentials_issued: false\n  third_party_delegation: false\n  headline: >-\n    No API key, no OAuth client registration, no token endpoint and no scope\n    surface exists for any SaskPower data. The open feeds need nothing; the\n    customer data behind MySaskPower is reachable only by the account holder\n    signing in through Azure AD B2C in a browser.\nschemes:\n- name: none\n  type: none\n\
  \  applies_to:\n  - saskpower:saskpower-power-use-dashboard-data\n  - saskpower:saskpower-planned-outages-rss-feed\n  - saskpower:saskpower-live-outage-json-feed\n  - saskpower:saskpower-outage-map-kml-feed\n  - saskpower:saskpower-smart-meter-installation-map-kml-feed\n  detail: >-\n    Anonymous HTTPS GET. Verified 2026-07-27 against all five endpoints with no\n    Authorization header, no cookie, no API key and no Referer: every one returned\n    HTTP 200 with its full payload. No key, no signup, no quota and no published\n    rate limit. The endpoints do set a Sitecore SP_CACHE_KEY session cookie on the\n    response (path=/, secure, HttpOnly, SameSite=None) but do not require it on\n    the request.\n  cors: >-\n    No Access-Control-Allow-Origin header is returned, tested with an explicit\n    Origin: https://example.com. Browser-side third-party use is therefore blocked\n    by the same-origin policy; these feeds are reachable server-side only.\n- name: SaskPower.Azure.B2C\n  type:\
  \ openIdConnect\n  applies_to: MySaskPower customer portal (not an API)\n  identity_provider: Azure AD B2C, fronted by Sitecore Identity\n  evidence: >-\n    https://www.saskpower.com/profile/my-dashboard and\n    https://www.saskpower.com/Profile/My-Dashboard/My-Reports/Download-Data both\n    return a 519-byte auto-submitting HTML form POSTing to\n    /identity/externallogin?authenticationType=SaskPower.Azure.B2C with a\n    ReturnUrl back to the requested page. Confirmed 2026-07-27.\n  delegated_access: false\n  detail: >-\n    A human browser login, not an authorization surface. There is no client\n    registration, no consent screen offered to a third party, no scope vocabulary,\n    no token endpoint published, and no documented way for an application to be\n    authorized to read another person's data. A customer can reach an in-portal\n    \"Download Data\" report page (/Profile/My-Dashboard/My-Reports/Download-Data)\n    but no export format is advertised anywhere on the public\
  \ site and the page\n    itself is behind the login, so no format is recorded here.\n  session_endpoints_observed:\n  - /api/sitecore/B2CAuthentication/ExtendLoginCookie\n  - /api/sitecore/B2CAuthentication/Logout\n- name: Microsoft Entra ID (partner portal)\n  type: openIdConnect\n  applies_to: partner.saskpower.com\n  detail: >-\n    302s to login.microsoftonline.com, tenant\n    dbe9bd7b-4b3a-44b3-b358-e61ff34d58b2, response_type=code id_token,\n    scope=openid profile. Corporate partner SSO for contractors and vendors, not a\n    developer portal and not an API gate.\n- name: TIBCO Cloud API Management (Mashery) gateway\n  type: unknown\n  applies_to: api.saskpower.com\n  detail: >-\n    The gateway is live — CNAME saskpower1.api.mashery.com — but no service is\n    mapped to any public path: every path probed returns HTTP 596 with\n    x-mashery-error-code ERR_596_SERVICE_NOT_FOUND from Server: Mashery Proxy.\n    Mashery's normal auth model is an api_key/sig query pair, but nothing\
  \ is\n    exposed to confirm which scheme any real service behind it uses, so the type\n    is recorded as unknown rather than guessed. The developer portal that would\n    have issued keys, api-info.saskpower.com, is NXDOMAIN.\ndiscovery:\n  openid_configuration: not served on any SaskPower host (see well-known/saskpower-well-known.yml)\n  oauth_authorization_server: not served\n  oauth_protected_resource: not served\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saskpower/refs/heads/main/authentication/saskpower-authentication.yml
summary_line: none/oidc-human-login · 4 schemes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Smart Metering
- Crown Corporation
- Outages
- Renewables
- Open Data
---
