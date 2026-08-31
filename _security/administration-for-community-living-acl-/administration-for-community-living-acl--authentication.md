---
api_key_in: []
auth_types: []
description: ACL publishes no developer authentication documentation. Two live ACL API hosts were discovered by reading the public front-end bundles of ACL's own web properties; this artifact records the authentication model each one actually enforces, observed on the wire. Neither surface has a signup, a key-issuance flow, or a documented auth page.
kind: authentication
layout: security
method: probed
name: Administration For Community Living Acl  Authentication
name_suffix: Authentication
oauth_flows: []
overview: Administration for Community Living (ACL) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Administration for Community Living (ACL)
provider_slug: administration-for-community-living-acl-
scheme_count: 2
schemes:
- api: AGID Program Data API
  base: https://sic.acl.gov/p-agid-ui-fn
  documented: false
  evidence:
    request: POST https://sic.acl.gov/p-agid-ui-fn/GetDataSets with no key
    response_header: 'www-authenticate: AzureApiManagementKey realm="https://p-acl-apim.azure-api.net/p-agid-ui-fn", name="Ocp-Apim-Subscription-Key", type="header"'
    status: 401
  host: sic.acl.gov
  id: agid-apim-subscription-key
  in: header
  name: Ocp-Apim-Subscription-Key
  note: The subscription key the AGID web app uses is compiled into its public JavaScript bundle and is therefore shipped to every browser that loads agid.acl.gov. Its value is deliberately NOT recorded in this repository. There is no published process by which a third party can obtain a key of their own, so this is a browser-embedded key rather than a developer credential.
  provider_stack: Azure API Management
  realm: https://p-acl-apim.azure-api.net/p-agid-ui-fn
  self_service_signup: false
  type: apiKey
- api: Eldercare Locator Content API
  base: https://ehc.acl.gov/api
  documented: false
  evidence:
    content_type: application/json; charset=utf-8
    request: GET https://ehc.acl.gov/api/eldercareglobal with no credentials
    status: 200
  host: ehc.acl.gov
  id: eldercare-anonymous
  note: Strapi 5 headless CMS. The eldercareglobal collection is readable anonymously; other Strapi collection names probed (pages, articles, topics, resources) return 404, so the public role exposes a narrow allowlist rather than the whole content model.
  self_service_signup: false
  type: none
slug: administration-for-community-living-acl--authentication
source_filename: administration-for-community-living-acl--authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Administration for Community Living (ACL)\nproviderId: administration-for-community-living-acl-\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes of https://sic.acl.gov/p-agid-ui-fn and https://ehc.acl.gov/api,\n  plus the AGID front-end bundle https://agid.acl.gov/assets/index-2c03a0f9.js\n  which declares the gateway base URL and header name.\ndescription: >-\n  ACL publishes no developer authentication documentation. Two live ACL API hosts\n  were discovered by reading the public front-end bundles of ACL's own web\n  properties; this artifact records the authentication model each one actually\n  enforces, observed on the wire. Neither surface has a signup, a key-issuance\n  flow, or a documented auth page.\nschemes:\n  - id: agid-apim-subscription-key\n    api: AGID Program Data API\n    host: sic.acl.gov\n    base: https://sic.acl.gov/p-agid-ui-fn\n    type: apiKey\n    in:\
  \ header\n    name: Ocp-Apim-Subscription-Key\n    provider_stack: Azure API Management\n    realm: https://p-acl-apim.azure-api.net/p-agid-ui-fn\n    documented: false\n    self_service_signup: false\n    evidence:\n      request: POST https://sic.acl.gov/p-agid-ui-fn/GetDataSets with no key\n      status: 401\n      response_header: >-\n        www-authenticate: AzureApiManagementKey\n        realm=\"https://p-acl-apim.azure-api.net/p-agid-ui-fn\",\n        name=\"Ocp-Apim-Subscription-Key\", type=\"header\"\n    note: >-\n      The subscription key the AGID web app uses is compiled into its public\n      JavaScript bundle and is therefore shipped to every browser that loads\n      agid.acl.gov. Its value is deliberately NOT recorded in this repository.\n      There is no published process by which a third party can obtain a key of\n      their own, so this is a browser-embedded key rather than a developer\n      credential.\n  - id: eldercare-anonymous\n    api: Eldercare Locator Content\
  \ API\n    host: ehc.acl.gov\n    base: https://ehc.acl.gov/api\n    type: none\n    documented: false\n    self_service_signup: false\n    evidence:\n      request: GET https://ehc.acl.gov/api/eldercareglobal with no credentials\n      status: 200\n      content_type: application/json; charset=utf-8\n    note: >-\n      Strapi 5 headless CMS. The eldercareglobal collection is readable\n      anonymously; other Strapi collection names probed (pages, articles, topics,\n      resources) return 404, so the public role exposes a narrow allowlist rather\n      than the whole content model.\noauth2: false\nopenid_connect: false\nmutual_tls: false\noauth_discovery:\n  probed:\n    - url: https://sic.acl.gov/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://sic.acl.gov/.well-known/openid-configuration\n      status: 404\n    - url: https://acl.gov/.well-known/openid-configuration\n      status: 404\ndocs: null\ndocs_note: No ACL authentication or developer-credential\
  \ documentation was found on any ACL host.\nmaintainers:\n  - FN: Kin Lane\n    X-twitter: apievangelist\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administration-for-community-living-acl-/refs/heads/main/authentication/administration-for-community-living-acl--authentication.yml
summary_line: 2 schemes
tags:
- Aging
- Federal-Government
- Healthcare
- Disability
- Independent Living
- Open Data
- Social Services
---
