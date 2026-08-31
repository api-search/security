---
api_key_in: []
api_specs:
- filename: hkust-path-advisor-openapi.yml
  format: yaml
  label: HKUST Path Advisor API
  slug: path-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/openapi/hkust-path-advisor-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hkust Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hong Kong University of Science and Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hong Kong University of Science and Technology
provider_slug: hkust
scheme_count: 0
schemes: []
slug: hkust-authentication
source_filename: hkust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Hong Kong University of Science and Technology — authentication across surfaces\nprovider: Hong Kong University of Science and Technology\nproviderId: hkust\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live unauthenticated probes on 2026-08-30 plus HKUST's own published instructions on\n  itso.hkust.edu.hk. Each entry records the operator of the surface, because for a\n  university the authentication story is mostly somebody else's.\nsurfaces:\n  - surface: HKUST Path Advisor API\n    baseURL: https://pathadvisor.ust.hk/api\n    x-operator: institution\n    scheme: none\n    description: >-\n      No authentication of any kind on the public routes. Access-Control-Allow-Origin is *,\n      so the API is callable directly from any browser origin. Verified by unauthenticated\n      200 responses from /floors, /buildings, /tags, /nodes and /nodes/{id}.\n    exception:\n      route: /connectors\n      status: 401\n      body: '{\"error\":{\"message\":\"Authorization\
  \ failed\"}}'\n      note: >-\n        Gated, with no WWW-Authenticate header and no published enrollment path. The scheme\n        is unknown and is deliberately not guessed at.\n    evidence:\n      - url: https://pathadvisor.ust.hk/api/floors\n        status: 200\n      - url: https://pathadvisor.ust.hk/api/connectors\n        status: 401\n  - surface: HKUST API Gateway (Azure API Management)\n    baseURL: https://hkust.azure-api.net\n    x-operator: tenant\n    scheme: apiKey\n    parameter: X-Apim-Subscription-Key\n    in: header\n    description: >-\n      Azure API Management subscription key, passed as a request header. HKUST documents the\n      header name and the flow explicitly: sign up at the HKUST API Portal with an ITSO\n      account, subscribe to a Product such as \"IoT Sensor Data\", and a key is emailed after\n      the request is reviewed and approved. Enrollment therefore requires HKUST affiliation\n      and human approval — this is not a self-service public API.\n\
  \    enrollment: https://hkust.developer.azure-api.net/signup\n    documentation: https://itso.hkust.edu.hk/services/it-infrastructure/smart-campus-infrastructure/open-data-platform/retrieve-iot-data-api\n    evidence:\n      - url: https://hkust.azure-api.net/sensor-data/_search\n        status: 401\n        body: 'Access denied due to missing subscription key.'\n      - url: https://hkust.azure-api.net/sensor-inventory/_search?q=location:LTL\n        status: 401\n  - surface: HKUST Shibboleth Identity Provider\n    entityID: https://idp.ust.hk/idp/shibboleth\n    x-operator: institution\n    scheme: SAML 2.0 / Shibboleth\n    description: >-\n      The institution's own SAML 2.0 identity provider — the authentication surface HKUST\n      genuinely operates itself. Asserts the scopes ust.hk, connect.ust.hk and alumni.ust.hk.\n      Supports SAML 2.0 HTTP-POST, HTTP-Redirect and SOAP/ECP bindings plus the legacy\n      Shibboleth 1.0 profile. Registered by the Hong Kong Access Federation\
  \ and published\n      into eduGAIN, carrying the REFEDS Research & Scholarship and SIRTFI entity categories.\n    endpoints:\n      - https://idp.ust.hk/idp/profile/SAML2/POST/SSO\n      - https://idp.ust.hk/idp/profile/SAML2/Redirect/SSO\n      - https://idp.ust.hk/idp/profile/SAML2/SOAP/ECP\n    securityContact: security@ust.hk\n    evidence:\n      - url: https://idp.ust.hk/idp/shibboleth\n        status: 200\n      - url: https://technical.edugain.org/api.php?action=show_entity&entityid=https://idp.ust.hk/idp/shibboleth\n        status: 200\n  - surface: DataSpace@HKUST (Dataverse Native API)\n    baseURL: https://dataspace.hkust.edu.hk/api\n    x-operator: institution\n    scheme: apiKey\n    parameter: X-Dataverse-key\n    in: header\n    description: >-\n      Read access to published datasets is unauthenticated — /api/info/version and\n      /api/search answered without credentials. Write and administrative operations use the\n      upstream Dataverse X-Dataverse-key header. The\
  \ authentication contract is the Dataverse\n      project's, not HKUST's; HKUST operates the deployment on its own domain and hardware.\n    evidence:\n      - url: https://dataspace.hkust.edu.hk/api/info/version\n        status: 200\n      - url: https://dataspace.hkust.edu.hk/api/search?q=*&type=dataset&per_page=1\n        status: 200\nnotFound:\n  - No OAuth 2.0 or OpenID Connect authorization server is published on any HKUST host probed.\n  - No .well-known/security.txt on www.ust.hk, itso.hkust.edu.hk or dataspace.hkust.edu.hk (404).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkust/refs/heads/main/authentication/hkust-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- Hong Kong
- China
- Research Data
- Open Data
- Identity Federation
- Course Catalog
- Library
- Smart Campus
- API Gateway
- Wayfinding
---
