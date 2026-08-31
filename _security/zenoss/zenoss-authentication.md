---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Virtana Service Observability API (formerly the Zenoss Cloud API). There are three distinct schemes across two API generations: the /v1 services take a long-lived key in a zenoss-api-key header, the legacy Collection Zone router API takes a key in a DIFFERENTLY NAMED z-api-key header, and on-premises Resource Manager router calls use HTTP Basic. There is no OAuth 2.0 or OpenID Connect flow on any API surface. OIDC, SAML and LDAP exist on the Zenoss/Virtana platform for interactive single sign-on to the web application, not for API clients.'
kind: authentication
layout: security
method: searched
name: Zenoss Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenoss declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Zenoss
provider_slug: zenoss
scheme_count: 3
schemes:
- applies_to:
  - REST /v1 services
  - gRPC DataReceiverService / DataRegistryService
  - OpenTelemetry OTLP metric export
  description: Long-lived authentication key issued from ADMIN > API Clients. Sent in the zenoss-api-key header of every request. Applies to both the REST/JSON services and the gRPC data receiver, and to the OpenTelemetry OTLP exporter (header zenoss-api-key=YOUR-ZENOSS-API-KEY).
  id: zenoss-api-key
  in: header
  name: zenoss-api-key
  source: https://docs.zenoss.io/api/zenoss-api.html
  type: apiKey
- applies_to:
  - POST /cz0/zport/dmd/<router> on a Collection Zone host
  description: Authentication key for the Zenoss API for Collection Zone and Resource Manager (the JSON router API). Note the header name differs from the /v1 services — z-api-key, not zenoss-api-key. Collection Zone keys are created by users on their Account Settings page and inherit the creating user's Collection Zone roles.
  id: z-api-key
  in: header
  name: z-api-key
  source: https://docs.zenoss.com/api/how-to/use-curl.html
  type: apiKey
- applies_to:
  - POST /zport/dmd/<router> on a Resource Manager host
  description: HTTP Basic authentication (api-username:api-password) for on-premises Zenoss Resource Manager / Service Dynamics router calls. Documented as `-u "api-username:api-password"` against https://<host>/zport/dmd/<router>.
  id: basic-auth
  scheme: basic
  source: https://docs.zenoss.com/api/how-to/use-curl.html
  type: http
slug: zenoss-authentication
source_filename: zenoss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.zenoss.io/admin/clients/zenoss-api.html\ndocs:\n  - https://docs.zenoss.io/api/zenoss-api.html\n  - https://docs.zenoss.io/admin/clients/zenoss-api.html\n  - https://docs.zenoss.io/admin/clients/cz-api.html\n  - https://www.virtana.com/trust/\n  - https://docs.zenoss.com/api/how-to/use-curl.html\nprovider: Zenoss\nproviderId: zenoss\ndescription: >-\n  Authentication profile for the Virtana Service Observability API (formerly the Zenoss Cloud API).\n  There are three distinct schemes across two API generations: the /v1 services take a long-lived key\n  in a zenoss-api-key header, the legacy Collection Zone router API takes a key in a DIFFERENTLY NAMED\n  z-api-key header, and on-premises Resource Manager router calls use HTTP Basic. There is no OAuth\n  2.0 or OpenID Connect flow on any API surface. OIDC, SAML and LDAP exist on the\n  Zenoss/Virtana platform for interactive single sign-on to the web application,\
  \ not for API clients.\nschemes:\n  - id: zenoss-api-key\n    type: apiKey\n    in: header\n    name: zenoss-api-key\n    description: >-\n      Long-lived authentication key issued from ADMIN > API Clients. Sent in the zenoss-api-key header\n      of every request. Applies to both the REST/JSON services and the gRPC data receiver, and to the\n      OpenTelemetry OTLP exporter (header zenoss-api-key=YOUR-ZENOSS-API-KEY).\n    applies_to:\n      - REST /v1 services\n      - gRPC DataReceiverService / DataRegistryService\n      - OpenTelemetry OTLP metric export\n    source: https://docs.zenoss.io/api/zenoss-api.html\n  - id: z-api-key\n    type: apiKey\n    in: header\n    name: z-api-key\n    description: >-\n      Authentication key for the Zenoss API for Collection Zone and Resource Manager (the JSON router\n      API). Note the header name differs from the /v1 services — z-api-key, not zenoss-api-key.\n      Collection Zone keys are created by users on their Account Settings page and\
  \ inherit the\n      creating user's Collection Zone roles.\n    applies_to:\n      - POST /cz0/zport/dmd/<router> on a Collection Zone host\n    source: https://docs.zenoss.com/api/how-to/use-curl.html\n  - id: basic-auth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication (api-username:api-password) for on-premises Zenoss Resource Manager /\n      Service Dynamics router calls. Documented as `-u \"api-username:api-password\"` against\n      https://<host>/zport/dmd/<router>.\n    applies_to:\n      - POST /zport/dmd/<router> on a Resource Manager host\n    source: https://docs.zenoss.com/api/how-to/use-curl.html\nkey_types:\n  - name: User Management API\n    grants: The user management service (/v1/user-mgmt/*).\n    source: https://docs.zenoss.io/admin/clients/zenoss-api.html\n  - name: User API\n    grants: >-\n      Most general user operations. Required to interact with the model context API — entity\n      management, custom properties, production\
  \ state and priority, entity activity and schema ID.\n    source: https://docs.zenoss.io/admin/clients/zenoss-api.html\n  - name: Streaming Data Ingest API\n    grants: All Virtana Service Observability API services except the User and User Management sets.\n    source: https://docs.zenoss.io/admin/clients/zenoss-api.html\n  - name: Collection Zone API key\n    grants: >-\n      The legacy Collection Zone API. Carries only the permissions of the creating user's Collection\n      Zone roles, and those permissions change when the user's roles change.\n    source: https://docs.zenoss.io/admin/clients/cz-api.html\nkey_management:\n  issuer_ui: ADMIN > API Clients (Virtana Service Observability console)\n  required_role: Key Administrator or Manager (Key Creator for Collection Zone keys)\n  keys_per_client: 200\n  cz_keys_per_user: 130\n  retrievable_after_creation: false\n  rotation: >-\n    Keys cannot be retrieved after creation; a lost key must be deleted and regenerated. Deleting a\n \
  \   key or its parent API Client denies access to clients using it within 60 seconds.\n  expiry: >-\n    Keys do not expire, and are not revoked when the creating user's account is removed or their\n    Key Creator role is withdrawn — revocation is manual.\n  audit: API Client names are written to audit logs on every update made through the API.\n  source: https://docs.zenoss.io/admin/clients/zenoss-api.html\nsso:\n  applies_to: Interactive sign-in to the Virtana/Zenoss platform, not to API clients.\n  protocols:\n    - LDAP\n    - SAML\n    - OIDC\n  mfa: Virtana states multi-factor authentication is used on all systems, for all access points.\n  source: https://www.virtana.com/trust/\noauth2: false\nopenid_connect_api: false\nmutual_tls: false\ntransport:\n  https_required: true\n  note: All API endpoints require HTTPS; the docs state all services require encryption.\nunauthenticated_status_codes:\n  - code: 401\n    meaning: missing or invalid authentication key\n  - code: 500\n   \
  \ meaning: >-\n      Documented on some resources as \"missing or invalid authentication key\" — an inconsistency in\n      the published status-code tables, recorded as found rather than corrected.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenoss/refs/heads/main/authentication/zenoss-authentication.yml
summary_line: 3 schemes
tags:
- AIOps
- Monitoring
- Observability
- Infrastructure
- Event Management
- Hybrid Cloud
- OpenTelemetry
- gRPC
- Metrics
---
