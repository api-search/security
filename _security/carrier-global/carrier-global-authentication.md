---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: carrier-global-lynx-fleet-api-openapi.yaml
  format: yaml
  label: Carrier Lynx Fleet API
  slug: lynx-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carrier-global/refs/heads/main/openapi/carrier-global-lynx-fleet-api-openapi.yaml
- filename: carrier-global-lynx-2way-command-api-openapi.yaml
  format: yaml
  label: Carrier Lynx 2-way Command API
  slug: lynx-2way-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carrier-global/refs/heads/main/openapi/carrier-global-lynx-2way-command-api-openapi.yaml
- filename: carrier-global-lynx-container-api-openapi.yaml
  format: yaml
  label: Carrier Lynx Container API
  slug: lynx-container-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carrier-global/refs/heads/main/openapi/carrier-global-lynx-container-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Carrier Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carrier Global secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Carrier Global
provider_slug: carrier-global
scheme_count: 1
schemes:
- applied: global
  failure_modes:
  - meaning: Invalid API key provided, or API key not provided
    status: 401
  - meaning: API Key doesn't have permission to perform requests
    status: 403
  in: header
  name: x-lynx-api-key
  obtaining_credentials: '"Admins can obtain an API key from the account menu in the Lynx Fleet portal. Click on your name in the Lynx Fleet header and select the External API Key option. You could also reach out to Lynx API Support to get your API Key." (published guide, verbatim)'
  parameter: x-lynx-api-key
  rotation: '"If you suspect your API key has been compromised, request a new key from the External API Key option within Lynx Fleet." (published guide, verbatim)'
  scoping: 'The key is tenant-scoped: "The Lynx API Key links a tenant to assets that the tenant has access to." API Configuration determines which tenants, assets and data types (GPS, temperature, door-open events) a given client may read, and must be in place before any call returns data.'
  sources:
  - openapi/carrier-global-lynx-fleet-api-openapi.yaml
  - openapi/carrier-global-lynx-2way-command-api-openapi.yaml
  - openapi/carrier-global-lynx-container-api-openapi.yaml
  transport: '"All requests need to be made over HTTPS. Calls made over regular HTTP will fail. Requests made without authentication will also fail." Best practices additionally require TLS 1.2 or higher and server-certificate validation.'
  type: apiKey
slug: carrier-global-authentication
source_filename: carrier-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://api.portal.fleet.lynx.carrier.io/public/graphql (getPublicProductInfo →\n  guide.gettingStarted.authentication), plus the securitySchemes block of all three\n  published contracts in openapi/\ndocs: https://doc-api.fleet.lynx.carrier.io/api-documentation\nprovider: Carrier Global\nproviderId: carrier-global\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Every published Carrier Lynx contract authenticates the same way: a single\n    tenant-scoped API key in the x-lynx-api-key request header, applied globally via a\n    root-level security requirement. There is no OAuth surface on the API itself, so no\n    scopes/ artifact is written. The Lynx Fleet WEB portal signs users in through\n    Carrier's own Okta tenant (OIDC) — that is human SSO for the UI, not API auth, and\n    is recorded separately in well-known/.\nschemes:\n\
  \  - name: x-lynx-api-key\n    type: apiKey\n    in: header\n    parameter: x-lynx-api-key\n    applied: global\n    sources:\n      - openapi/carrier-global-lynx-fleet-api-openapi.yaml\n      - openapi/carrier-global-lynx-2way-command-api-openapi.yaml\n      - openapi/carrier-global-lynx-container-api-openapi.yaml\n    obtaining_credentials: >-\n      \"Admins can obtain an API key from the account menu in the Lynx Fleet portal.\n      Click on your name in the Lynx Fleet header and select the External API Key\n      option. You could also reach out to Lynx API Support to get your API Key.\"\n      (published guide, verbatim)\n    rotation: >-\n      \"If you suspect your API key has been compromised, request a new key from the\n      External API Key option within Lynx Fleet.\" (published guide, verbatim)\n    transport: >-\n      \"All requests need to be made over HTTPS. Calls made over regular HTTP will fail.\n      Requests made without authentication will also fail.\" Best practices\
  \ additionally\n      require TLS 1.2 or higher and server-certificate validation.\n    scoping: >-\n      The key is tenant-scoped: \"The Lynx API Key links a tenant to assets that the\n      tenant has access to.\" API Configuration determines which tenants, assets and\n      data types (GPS, temperature, door-open events) a given client may read, and must\n      be in place before any call returns data.\n    failure_modes:\n      - status: 401\n        meaning: Invalid API key provided, or API key not provided\n      - status: 403\n        meaning: API Key doesn't have permission to perform requests\nidentity_surfaces:\n  - name: Lynx Fleet portal SSO\n    kind: oidc\n    issuer: https://carrier.okta.com/oauth2/ausezsnschc0QFWkt4x7\n    discovery: well-known/carrier-global-okta-lynx-app-openid-configuration.json\n    applies_to: human sign-in to the Lynx Fleet portal and Dev Portal\n    applies_to_api: false\n    note: >-\n      Named as REACT_APP_OKTA_ISSUER in the Dev Portal's own\
  \ published JavaScript\n      bundle. The Dev Portal integration guide also refers to signing in \"using SAML\n      credentials\".\nprerequisites:\n  - You must obtain a valid API key before integration; it must be included in the\n    x-lynx-api-key header of every request.\n  - Your subscription plan must support Pull API access.\n  - Outbound IPs may need whitelisting where Lynx enforces IP restrictions (documented\n    as optional, typically required in production).\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrier-global/refs/heads/main/authentication/carrier-global-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- HVAC
- Cold Chain
- Telematics
- Building Automation
- IoT
- Refrigeration
- Fortune 500
---
