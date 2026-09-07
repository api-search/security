---
anonymous_access: false
api_key_in: []
api_specs:
- filename: workspot-control-openapi-original.json
  format: json
  label: Workspot Control REST API
  slug: control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspot/refs/heads/main/openapi/workspot-control-openapi-original.json
auth_types:
- oauth2
- http
- hmac
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Workspot Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Workspot secures its APIs with oauth2, http, and hmac across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Workspot
provider_slug: workspot
scheme_count: 3
schemes:
- api: Workspot Control REST API
  client_authentication: HTTP Basic — the string "ClientID:ClientSecret" base64-encoded into the Authorization header. Client ID and Client Secret are issued in Workspot Control under Setup > API and can be regenerated at any time, which immediately invalidates the previous pair.
  flow: password
  name: Control API OAuth 2.0 (resource owner password credentials)
  regional_token_urls:
  - https://api.us.workspot.com/oauth/token
  - https://api.eu.workspot.com/oauth/token
  scopes: []
  scopes_note: Workspot documents no OAuth scope surface for the Control API. Authorization is carried by the Control administrator role, not by scopes, so no scopes/ artifact is emitted.
  source: https://docs.workspot.com/docs/using-the-workspot-control-api
  token_lifetime: 3600 seconds (one hour); re-run the token call to obtain a new one
  token_placement: 'Authorization: Bearer <access_token>'
  token_url: https://api.workspot.com/oauth/token
  type: oauth2
  user_credentials: grant_type=password with the username and password of a Workspot Control administrator account, posted as form parameters alongside the Basic client header.
- api: Workspot Control REST API
  description: Mandatory alternative for tenants configured as Entra-ID-only. The administrator sets Setup > API > Auth Type to "Azure AD Token (Entra ID)", at which point the Control Client ID and Client Secret are no longer used and no Control administrator credentials are sent. The caller obtains an access token from Entra ID for the "Workspot" Enterprise Application registered in the tenant and presents it as a bearer token.
  flow: azure-ad-token
  name: Microsoft Entra ID token
  requires:
  - Workspot registered as an Enterprise Application in the Entra ID tenant
  - the Enterprise Application's Application ID
  - the Entra ID Tenant ID
  source: https://docs.workspot.com/docs/using-entra-id-authentication-with-the-control-api
  type: oauth2
- algorithm: HMAC-SHA256
  api: Workspot SIEM (Splunk) Events API
  credentials: A Key Id and Secret Key issued in Workspot Control under Setup > Splunk, together with the tenant-specific Control Splunk API URL shown on the same page.
  description: Selected parts of the request are concatenated into a canonical string, a MAC is computed over it with the Secret Key using HMAC-SHA256, base64-encoded, and combined with the key identifier in the Authorization header.
  header: 'Authorization: WSEvents <keyId>:<base64(HMAC-SHA256(canonical_string, secretKey))>'
  name: WSEvents HMAC-SHA256
  scheme: WSEvents
  source: https://docs.workspot.com/docs/workspot-splunksiem-api-user-guide
  type: hmac
slug: workspot-authentication
source_filename: workspot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://docs.workspot.com/docs/using-the-workspot-control-api\ndocs: https://docs.workspot.com/docs/using-the-workspot-control-api\nalso: https://docs.workspot.com/docs/using-entra-id-authentication-with-the-control-api\nsummary:\n  types: [oauth2, http, hmac]\n  api_key_in: []\n  oauth2_flows: [password]\n  note: >-\n    The published Swagger 2.0 document declares NO securityDefinitions at all — the\n    mechanical derive pass found zero schemes across 105 operations. Every scheme below is\n    read from Workspot's own documentation, which is why this file is method: searched.\n    That absence is itself a finding: an agent reading only the machine-readable contract\n    cannot discover how to authenticate.\nschemes:\n- name: Control API OAuth 2.0 (resource owner password credentials)\n  api: Workspot Control REST API\n  type: oauth2\n  flow: password\n  token_url: https://api.workspot.com/oauth/token\n  regional_token_urls:\n\
  \  - https://api.us.workspot.com/oauth/token\n  - https://api.eu.workspot.com/oauth/token\n  client_authentication: >-\n    HTTP Basic — the string \"ClientID:ClientSecret\" base64-encoded into the Authorization\n    header. Client ID and Client Secret are issued in Workspot Control under Setup > API and\n    can be regenerated at any time, which immediately invalidates the previous pair.\n  user_credentials: >-\n    grant_type=password with the username and password of a Workspot Control administrator\n    account, posted as form parameters alongside the Basic client header.\n  token_placement: 'Authorization: Bearer <access_token>'\n  token_lifetime: 3600 seconds (one hour); re-run the token call to obtain a new one\n  scopes: []\n  scopes_note: >-\n    Workspot documents no OAuth scope surface for the Control API. Authorization is carried\n    by the Control administrator role, not by scopes, so no scopes/ artifact is emitted.\n  source: https://docs.workspot.com/docs/using-the-workspot-control-api\n\
  - name: Microsoft Entra ID token\n  api: Workspot Control REST API\n  type: oauth2\n  flow: azure-ad-token\n  description: >-\n    Mandatory alternative for tenants configured as Entra-ID-only. The administrator sets\n    Setup > API > Auth Type to \"Azure AD Token (Entra ID)\", at which point the Control Client\n    ID and Client Secret are no longer used and no Control administrator credentials are\n    sent. The caller obtains an access token from Entra ID for the \"Workspot\" Enterprise\n    Application registered in the tenant and presents it as a bearer token.\n  requires:\n  - Workspot registered as an Enterprise Application in the Entra ID tenant\n  - the Enterprise Application's Application ID\n  - the Entra ID Tenant ID\n  source: https://docs.workspot.com/docs/using-entra-id-authentication-with-the-control-api\n- name: WSEvents HMAC-SHA256\n  api: Workspot SIEM (Splunk) Events API\n  type: hmac\n  scheme: WSEvents\n  algorithm: HMAC-SHA256\n  header: 'Authorization: WSEvents\
  \ <keyId>:<base64(HMAC-SHA256(canonical_string, secretKey))>'\n  credentials: >-\n    A Key Id and Secret Key issued in Workspot Control under Setup > Splunk, together with\n    the tenant-specific Control Splunk API URL shown on the same page.\n  description: >-\n    Selected parts of the request are concatenated into a canonical string, a MAC is computed\n    over it with the Secret Key using HMAC-SHA256, base64-encoded, and combined with the key\n    identifier in the Authorization header.\n  source: https://docs.workspot.com/docs/workspot-splunksiem-api-user-guide\nenablement:\n  note: >-\n    API access is enabled by default for new customers; older tenants may need to contact\n    Workspot Support to have it enabled. When enabled, a \"Setup > API\" tab appears in Control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workspot/refs/heads/main/authentication/workspot-authentication.yml
summary_line: oauth2/http/hmac · 3 schemes
tags:
- Virtual Desktop Infrastructure
- Desktop as a Service
- Cloud PC
- End User Computing
- Cloud Infrastructure
- Enterprise IT
- Workspace Management
- SaaS
---
