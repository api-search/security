---
api_key_in:
- header
- query
api_specs:
- filename: T17KeScV
  format: yaml
  label: Appgain OmniChannel Messaging API
  slug: appgain-omnichannel-messaging-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/4679101/T17KeScV?version=latest
- filename: appgain-omnichannel.postman_collection.json
  format: json
  label: Appgain Notify API
  slug: appgain-notify-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/appgain/refs/heads/main/postman/appgain-omnichannel.postman_collection.json
- filename: appgain-omnichannel.postman_collection.json
  format: json
  label: Appgain Automator API
  slug: appgain-automator-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/appgain/refs/heads/main/postman/appgain-omnichannel.postman_collection.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appgain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appgain secures its APIs with apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Appgain
provider_slug: appgain
scheme_count: 6
schemes:
- aliases_observed:
  - appapikey
  description: Per-project application API key. The primary credential for every messaging, smart-link, media and event-logging call. Issued in the Appgain dashboard under Project Settings -> API and SDK Keys.
  in: header
  name: appApiKey
  parameter_name: appApiKey
  sources:
  - postman/appgain-omnichannel.postman_collection.json
  - https://docs.appgain.io/restAPI/introduction/
  type: apiKey
  used_by_hosts:
  - api.appgain.io
  - notify.appgain.io
  - automator.appgain.io
  - '{account_subdomain}.appgain.io'
- description: The same project API key accepted as a URL query parameter on at least two published operations — GET /user_log_event/{projectId}/{userId} and DELETE /{projectId}/delete_media_files. Appgain publishes these forms itself; a credential in the query string is logged by proxies, gateways and browser history, so header placement should be preferred where both are accepted.
  in: query
  name: appApiKeyQuery
  parameter_name: appApiKey
  sources:
  - postman/appgain-omnichannel.postman_collection.json
  type: apiKey
- description: Parse Server application identifier. Required, together with the master key, on the two Parse cloud-function operations in the published collection (/functions/getUserInfo, /functions/logPurchase) against the per-account Appbackend server URL. Appgain's backend is built on the open-source Parse Server stack.
  in: header
  name: parseApplicationId
  parameter_name: x-parse-application-id
  sources:
  - postman/appgain-omnichannel.postman_collection.json
  type: apiKey
- description: Parse Server MASTER key. This is an unrestricted, full-privilege credential that bypasses Parse class-level permissions and ACLs — it is not an equivalent of the scoped project API key. Appgain's own published examples send it directly from the integration client, which means the documented path for logging a purchase or reading a user profile requires holding an admin-grade secret in the caller.
  in: header
  name: parseMasterKey
  parameter_name: x-parse-master-key
  risk: high
  sources:
  - postman/appgain-omnichannel.postman_collection.json
  type: apiKey
- bearer_format: JWT
  description: A vendor JWT carried IN ADDITION to appapikey on the WhatsApp Business API paths (POST /{projectId}/create_whatsapp_template and WHATSAPP sends). The token payload seen in Appgain's own n8n guide carries user_id, username, customer_id, send_message and reseller claims. It is not issued by any documented Appgain token endpoint; the docs do not say how an integrator obtains or refreshes it.
  name: whatsappAuthorization
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://docs.appgain.io/integrations/n8n-integration/
  type: http
- description: A second JWT header sent alongside Authorization on the WhatsApp template-creation call. Its issuance and lifetime are undocumented.
  in: header
  name: whatsappAuthToken
  parameter_name: authToken
  sources:
  - https://docs.appgain.io/integrations/n8n-integration/
  type: apiKey
slug: appgain-authentication
source_filename: appgain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  postman/appgain-omnichannel.postman_collection.json (verbatim public collection\n  4679101/T17KeScV) + https://docs.appgain.io/restAPI/introduction/ +\n  https://docs.appgain.io/integrations/n8n-integration/ + live unauthenticated probes\ndocs: https://docs.appgain.io/restAPI/introduction/\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  notes: >-\n    Appgain's REST surface is API-key only. A per-project application key is sent in\n    an `appApiKey` request header (lowercase `appapikey` in the notify.appgain.io\n    examples) and the tenant is selected by a `projectId` path segment. There is no\n    OAuth 2.0 authorization server, no OIDC discovery document, no token endpoint and\n    no scope surface anywhere in the published contract — /.well-known/oauth-authorization-server\n    and /.well-known/openid-configuration miss on every host\
  \ (see\n    well-known/appgain-well-known.yml). Two SECONDARY credential systems exist behind\n    the same platform: the Parse Server backend cloud functions, which take Parse\n    application-id/master-key headers, and the WhatsApp Business vendor path, which\n    additionally carries bearer-style JWTs. Neither is a scoped OAuth flow.\nschemes:\n- name: appApiKey\n  type: apiKey\n  in: header\n  parameter_name: appApiKey\n  aliases_observed: [appapikey]\n  description: >-\n    Per-project application API key. The primary credential for every messaging,\n    smart-link, media and event-logging call. Issued in the Appgain dashboard under\n    Project Settings -> API and SDK Keys.\n  used_by_hosts: [api.appgain.io, notify.appgain.io, automator.appgain.io, '{account_subdomain}.appgain.io']\n  sources: [postman/appgain-omnichannel.postman_collection.json, 'https://docs.appgain.io/restAPI/introduction/']\n- name: appApiKeyQuery\n  type: apiKey\n  in: query\n  parameter_name: appApiKey\n  description:\
  \ >-\n    The same project API key accepted as a URL query parameter on at least two\n    published operations — GET /user_log_event/{projectId}/{userId} and\n    DELETE /{projectId}/delete_media_files. Appgain publishes these forms itself; a\n    credential in the query string is logged by proxies, gateways and browser\n    history, so header placement should be preferred where both are accepted.\n  sources: [postman/appgain-omnichannel.postman_collection.json]\n- name: parseApplicationId\n  type: apiKey\n  in: header\n  parameter_name: x-parse-application-id\n  description: >-\n    Parse Server application identifier. Required, together with the master key,\n    on the two Parse cloud-function operations in the published collection\n    (/functions/getUserInfo, /functions/logPurchase) against the per-account\n    Appbackend server URL. Appgain's backend is built on the open-source Parse\n    Server stack.\n  sources: [postman/appgain-omnichannel.postman_collection.json]\n- name: parseMasterKey\n\
  \  type: apiKey\n  in: header\n  parameter_name: x-parse-master-key\n  description: >-\n    Parse Server MASTER key. This is an unrestricted, full-privilege credential that\n    bypasses Parse class-level permissions and ACLs — it is not an equivalent of the\n    scoped project API key. Appgain's own published examples send it directly from\n    the integration client, which means the documented path for logging a purchase\n    or reading a user profile requires holding an admin-grade secret in the caller.\n  risk: high\n  sources: [postman/appgain-omnichannel.postman_collection.json]\n- name: whatsappAuthorization\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  parameter_name: Authorization\n  description: >-\n    A vendor JWT carried IN ADDITION to appapikey on the WhatsApp Business API paths\n    (POST /{projectId}/create_whatsapp_template and WHATSAPP sends). The token\n    payload seen in Appgain's own n8n guide carries user_id, username, customer_id,\n    send_message and\
  \ reseller claims. It is not issued by any documented Appgain\n    token endpoint; the docs do not say how an integrator obtains or refreshes it.\n  sources: ['https://docs.appgain.io/integrations/n8n-integration/']\n- name: whatsappAuthToken\n  type: apiKey\n  in: header\n  parameter_name: authToken\n  description: >-\n    A second JWT header sent alongside Authorization on the WhatsApp template-creation\n    call. Its issuance and lifetime are undocumented.\n  sources: ['https://docs.appgain.io/integrations/n8n-integration/']\npath_scoping:\n  parameter: projectId\n  location: path\n  description: >-\n    Tenancy is expressed in the path, not in the credential. Every operation is\n    scoped by a projectId that the caller supplies; the API key is bound to that\n    project.\n  examples:\n  - https://notify.appgain.io/{projectId}/send\n  - https://automator.appgain.io/automessages/{projectId}/firevent/{trigger}/{userId}\n  - https://{account_subdomain}.appgain.io/apps/{projectId}/smartlinks\n\
  credentials_source: Appgain dashboard -> Project Settings -> API and SDK Keys\nrotation:\n  documented: false\n  notes: No key-rotation, key-expiry or multi-key policy is published.\nfailure_behaviour:\n  method: probed\n  probed: '2026-08-13'\n  observations:\n  - host: automator.appgain.io\n    request: GET /automessages/{projectId}/firevent/{trigger}/{userId} with an invalid appApiKey\n    status: 401\n    body: '{\"status\": \"failed\", \"message\": \"Not Authorized Api Key\"}'\n  - host: api.appgain.io\n    request: GET /user_log_event/{projectId}/{userId}?appApiKey=<invalid>\n    status: 401\n    body: '{\"status\": \"failed\", \"message\": \"app API key or user authentication required\"}'\n  - host: notify.appgain.io\n    request: POST /{projectId}/send with an invalid appapikey\n    status: 500\n    body: '{\"exception\": \"''NoneType'' object has no attribute ''api_key''\", \"message\": \"something went wrong\", \"status\": \"Failed\"}'\n    note: >-\n      The send endpoint does\
  \ not return 401 for a bad credential. It returns HTTP 500\n      and echoes a server-side Python AttributeError back to the caller. An agent\n      cannot distinguish \"your key is wrong\" from \"the service is broken\" on the\n      single most important endpoint in the API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appgain/refs/heads/main/authentication/appgain-authentication.yml
summary_line: apiKey · 6 schemes
tags:
- Company
- Mobile Marketing
- Marketing Automation
- Omnichannel Messaging
- Push Notifications
- SMS
- Email
- WhatsApp
- Customer Data Platform
- Deep Linking
- Customer Engagement
- AI Agents
- Conversational AI
- MENA
---
