---
api_key_in: []
api_specs:
- filename: virtual-peaker-commands-api-openapi.yml
  format: yaml
  label: Virtual Peaker Commands API
  slug: virtual-peaker-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-commands-api-openapi.yml
- filename: virtual-peaker-devices-api-openapi.yml
  format: yaml
  label: Virtual Peaker Devices API
  slug: virtual-peaker-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-devices-api-openapi.yml
- filename: virtual-peaker-energy-interval-endpoint-api-openapi.yml
  format: yaml
  label: Virtual Peaker Energy Interval Endpoint API
  slug: virtual-peaker-energy-interval-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-energy-interval-endpoint-api-openapi.yml
- filename: virtual-peaker-group-management-api-openapi.yml
  format: yaml
  label: Virtual Peaker Group Management API
  slug: virtual-peaker-group-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-group-management-api-openapi.yml
- filename: virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
  format: yaml
  label: Virtual Peaker OAuth Device Discovery (Preferred) API
  slug: virtual-peaker-oauth-device-discovery-preferred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - End User App API
  slug: virtual-peaker-pairing-code-device-discovery-end-user-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - Utility Commissioned Installation API
  slug: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
- filename: virtual-peaker-publishing-api-openapi.yml
  format: yaml
  label: Virtual Peaker Publishing API
  slug: virtual-peaker-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-publishing-api-openapi.yml
auth_types:
- oauth2
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Virtual Peaker Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Virtual Peaker secures its APIs with oauth2 and hmac across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Virtual Peaker
provider_slug: virtual-peaker
scheme_count: 3
schemes:
- applies_to_operations: 16 of the 18 device-partner operations
  client_authentication: Send as Basic header (per Virtual Peaker's published Postman setup)
  credentials:
  - clientId
  - clientSecret
  credentials_note: program-specific, provided by the Device Partner
  direction: VPP -> Device Partner
  flows:
  - flow: clientCredentials
    scope_names:
    - basic_partner_read_write
    scopes: 1
    tokenUrl: https://example.com/oauth/token
    tokenUrl_note: Placeholder. The Device Partner (OEM) hosts the authorization server; the real token endpoint is exchanged during onboarding.
  name: device_partner_api_auth
  sources:
  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml
  type: oauth2
- applies_to_operations:
  - readCurrentUser
  - readCurrentUserDevices
  description: If using the OAuth onboarding method, this authentication method is used for the respective endpoints (published description). Used by the OAuth Device Discovery enrollment flow, where the homeowner logs in to the device partner and grants the VPP access to their devices. May reuse the client-credentials application or use separate credentials.
  direction: VPP -> Device Partner (homeowner-consented)
  flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    scope_names:
    - user_read
    scopes: 1
    tokenUrl: https://example.com/oauth/token
  name: device_partner_user_auth
  pkce: not specified in the specification
  sources:
  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml
  type: oauth2
- algorithm: HMAC-SHA256
  declared_in_spec: false
  direction: Device Partner -> VPP
  header: Authorization
  history: spec 1.2.0 clarified the header is `Authorization`, not `Authentication`
  key_material:
  - issued: when the utility program is set up
    name: PROGRAM_PUBLISH_SECRET
    used_by:
    - publishCommand
    - publishDeviceEnrollment
    - publishDevicePartnerDrivenEnrollment
  - issued: per device, delivered when the VPP calls modifySubscription at enrollment
    name: DEVICE_PUBLISH_SECRET
    used_by:
    - publishSignalSetting
    - publishDeviceCommand
  name: publish_hmac
  path_identifier: PROGRAM_PUBLISH_KEY (path parameter on every publishing endpoint)
  reference_implementation: 'const crypto = require(''crypto'');

    const computedHMAC = crypto.createHmac(''sha256'', secret).update(body).digest(''hex'');

    // Authorization: Publish ${computedHMAC}

    '
  signed_material: the raw JSON request body
  sources:
  - https://assets.virtualpeaker.io/gravity-connect/vp-api.html#section/Authentication
  - openapi/virtual-peaker-gravity-connect-vpp-api-openapi.yml
  type: hmac
  value_format: Publish <hex-hmac>
slug: virtual-peaker-authentication
source_filename: virtual-peaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\ndocs:\n- https://assets.virtualpeaker.io/gravity-connect/vp-api.html#section/Authentication\n- https://assets.virtualpeaker.io/gravity-connect/device-partner-api.html#section/Authentication\nnote: >-\n  Derived mechanically from the OpenAPI securitySchemes, then upgraded from the published\n  Authentication sections of both Gravity Connect guides. The upgrade matters: the VPP publishing\n  document declares an EMPTY components.securitySchemes and no security requirement, yet all five\n  of its operations are authenticated with an HMAC-SHA256 signature. A tool reading only the spec\n  would conclude that half of Gravity Connect is unauthenticated.\nsummary:\n  types:\n  - oauth2\n  - hmac\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  directions:\n  - direction: VPP -> Device Partner\n    model: oauth2\n  - direction: Device Partner ->\
  \ VPP\n    model: hmac-sha256 body signature\ncredential_issuance:\n  model: partner-only, per utility program\n  request: gravity-connect@virtual-peaker.com\n  self_serve: false\nschemes:\n- name: device_partner_api_auth\n  type: oauth2\n  direction: VPP -> Device Partner\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth/token\n    tokenUrl_note: >-\n      Placeholder. The Device Partner (OEM) hosts the authorization server; the real token endpoint\n      is exchanged during onboarding.\n    scopes: 1\n    scope_names: [basic_partner_read_write]\n  client_authentication: Send as Basic header (per Virtual Peaker's published Postman setup)\n  credentials: [clientId, clientSecret]\n  credentials_note: program-specific, provided by the Device Partner\n  applies_to_operations: 16 of the 18 device-partner operations\n  sources:\n  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n- name: device_partner_user_auth\n  type: oauth2\n  direction:\
  \ VPP -> Device Partner (homeowner-consented)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\n    scopes: 1\n    scope_names: [user_read]\n  description: >-\n    If using the OAuth onboarding method, this authentication method is used for the respective\n    endpoints (published description). Used by the OAuth Device Discovery enrollment flow, where\n    the homeowner logs in to the device partner and grants the VPP access to their devices. May\n    reuse the client-credentials application or use separate credentials.\n  applies_to_operations: [readCurrentUser, readCurrentUserDevices]\n  pkce: not specified in the specification\n  sources:\n  - openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml\n- name: publish_hmac\n  type: hmac\n  algorithm: HMAC-SHA256\n  direction: Device Partner -> VPP\n  declared_in_spec: false\n  header: Authorization\n  value_format: 'Publish <hex-hmac>'\n\
  \  signed_material: the raw JSON request body\n  key_material:\n  - name: PROGRAM_PUBLISH_SECRET\n    issued: when the utility program is set up\n    used_by: [publishCommand, publishDeviceEnrollment, publishDevicePartnerDrivenEnrollment]\n  - name: DEVICE_PUBLISH_SECRET\n    issued: per device, delivered when the VPP calls modifySubscription at enrollment\n    used_by: [publishSignalSetting, publishDeviceCommand]\n  path_identifier: PROGRAM_PUBLISH_KEY (path parameter on every publishing endpoint)\n  reference_implementation: |\n    const crypto = require('crypto');\n    const computedHMAC = crypto.createHmac('sha256', secret).update(body).digest('hex');\n    // Authorization: Publish ${computedHMAC}\n  history: spec 1.2.0 clarified the header is `Authorization`, not `Authentication`\n  sources:\n  - https://assets.virtualpeaker.io/gravity-connect/vp-api.html#section/Authentication\n  - openapi/virtual-peaker-gravity-connect-vpp-api-openapi.yml\ngaps:\n- the VPP publishing document declares\
  \ no securityScheme at all — see\n  overlays/virtual-peaker-gravity-connect-vpp-api-overlay.yaml for the recommended declaration\n- the root security requirement of the device-partner document references a scope\n  (device_partner_basic_auth) that no flow declares\n- no OIDC discovery, no RFC 8414 metadata, no PKCE requirement, no mTLS\n- no token lifetime, refresh or rotation policy is published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/authentication/virtual-peaker-authentication.yml
summary_line: oauth2/hmac · 3 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- Demand Response
- DER
- DERMS
- Virtual Power Plant
- EV Charging
- Smart Thermostats
- Energy Storage
---
