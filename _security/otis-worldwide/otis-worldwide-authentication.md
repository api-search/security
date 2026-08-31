---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Otis Worldwide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Otis Worldwide declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Otis Worldwide
provider_slug: otis-worldwide
scheme_count: 0
schemes: []
slug: otis-worldwide-authentication
source_filename: otis-worldwide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://www.otis.com/documents/256045/119472397/OID_Robot-Prodivers_Datasheet_InDesign_WHQ_English_Final.pdf/215d5e99-fd88-5502-aa1a-078c8c3b3eff?t=1655310590825\nauthentication:\n  slug: otis-worldwide\n  name: Otis Worldwide\n  summary: >-\n    Otis does not publish a machine-readable contract, so this profile is assembled from the\n    company's own published API data sheet and developer-portal pages rather than derived from an\n    OpenAPI securitySchemes block. Two layers stack: an Azure API Management subscription key\n    issued when a developer subscribes to an API product in the Otis Developer Portal, and OAuth 2.0\n    client-credentials tokens minted from a client-id / client-secret pair for the API itself.\n  docs:\n    - url: https://developers.otis.com/signup\n      note: Developer account sign-up; carries the Terms & Conditions for use of the Otis Developer Portal.\n      status: 200\n    - url: https://developers.otis.com/apis\n\
  \      note: >-\n        Portal API catalogue. Anonymous callers see zero APIs — the reference, including the\n        authoritative auth reference, requires a signed-in developer account with a subscribed\n        API product.\n      status: 200\n  schemes:\n    - id: otis-portal-subscription-key\n      type: apiKey\n      in: header\n      name: Ocp-Apim-Subscription-Key\n      applies_to: All APIs published through the Otis Developer Portal (Azure API Management)\n      description: >-\n        Otis's service-robot data sheet states \"Subscribe to the API product to request sandbox\n        access. A subscription key will be required for further operations.\" The portal is a\n        Microsoft Azure API Management instance (config.json managementApiUrl\n        apim-apip-prod-naa-7yxcbl5fhzara.management.azure-api.net), whose standard subscription-key\n        header is Ocp-Apim-Subscription-Key. The header NAME is inferred from the platform, not\n        stated by Otis; the requirement\
  \ for a subscription key is stated by Otis.\n      confidence: medium\n      evidence:\n        - >-\n          \"A subscription key will be required for further operations.\" — Otis Integrated Dispatch\n          Data Sheet for Service Robot Providers, GET STARTED section.\n        - https://developers.otis.com/config.json (HTTP 200, Azure APIM portal configuration)\n    - id: otis-oid-oauth2-client-credentials\n      type: oauth2\n      flow: clientCredentials\n      applies_to: Otis Integrated Dispatch (OID) API\n      description: >-\n        \"Client Authentication: Via client-id & client-secret. Authorization: OAuth 2.0 – client\n        credentials flow.\" Otis publishes the flow but not the token endpoint URL, the scope names,\n        or the token lifetime; all three are inside the gated portal reference.\n      token_endpoint: null\n      scopes: []\n      confidence: high\n      evidence:\n        - >-\n          \"API SECURITY — API Protocol: Secure Websockets; Encryption:\
  \ TLS 1.2, Data encryption at\n          rest and in transit; Client Authentication: Via client-id & client-secret; Authorization:\n          OAuth 2.0 – client credentials flow; Traffic Throttling: None\" — Otis Integrated Dispatch\n          Data Sheet for Service Robot Providers.\n  transport:\n    protocol: Secure WebSockets\n    tls: TLS 1.2\n    encryption_at_rest: true\n    note: >-\n      Otis states all API communication runs over an encrypted channel and all stored data is\n      encrypted at rest.\n  gaps:\n    - No OAuth 2.0 authorization-server metadata is published; /.well-known/oauth-authorization-server 404s on every Otis host probed.\n    - No token endpoint, scope list, or token lifetime is published outside the authenticated portal.\n    - No OpenAPI or AsyncAPI document is published, so securitySchemes cannot be derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otis-worldwide/refs/heads/main/authentication/otis-worldwide-authentication.yml
summary_line: 0 schemes
tags:
- Elevators
- Escalators
- Building Management
- Smart Buildings
- Internet of Things
- Robotics
- Building Automation
- Elevator Dispatch
- Industrial
- Manufacturing
---
