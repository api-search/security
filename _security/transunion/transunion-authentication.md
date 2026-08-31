---
api_key_in:
- query
api_specs:
- filename: transunion-authentication-service-api-openapi.yml
  format: yaml
  label: TransUnion Authentication Service API
  slug: transunion-authentication-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/openapi/transunion-authentication-service-api-openapi.yml
- filename: transunion-signing-api-openapi.yml
  format: yaml
  label: TransUnion Signing API
  slug: transunion-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/openapi/transunion-signing-api-openapi.yml
- filename: transunion-verification-api-openapi.yml
  format: yaml
  label: TransUnion Verification API
  slug: transunion-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/openapi/transunion-verification-api-openapi.yml
- filename: transunion-verification-service-api-openapi.yml
  format: yaml
  label: TransUnion Verification Service API
  slug: transunion-verification-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/openapi/transunion-verification-service-api-openapi.yml
- filename: transunion-verification-service-with-call-validation-treatment-cvt-api-openapi.yml
  format: yaml
  label: TransUnion Verification Service with Call Validation Treatment (CVT) API
  slug: transunion-verification-service-with-call-validation-treatment-cvt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/openapi/transunion-verification-service-with-call-validation-treatment-cvt-api-openapi.yml
auth_types:
- apiKey
- ip-allowlist
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Transunion Authentication
name_suffix: Authentication
oauth_flows: []
overview: TransUnion secures its APIs with apiKey, ip-allowlist, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TransUnion
provider_slug: transunion
scheme_count: 3
schemes:
- applies_to:
  - authn/identityj-j
  - authn/identitys-j
  - authn/identitys-s
  - authn/identitymps
  - authn/identitympj
  - verify/identityj-j
  - verify/identitys-j
  - verify/identitys-s
  - verify/identitycvt
  declared_in_spec_as: parameter
  description: '"If a RESTful API client chooses to use ''apiKey'' for authentication, an ''apiKey'' query parameter, with a pre-provisioned value, is validated to access API calls that are restricted." (info.description, verbatim)'
  in: query
  name: apiKey
  parameter: apiKey
  required: false
  sources:
  - openapi/transunion-trucontact-tcs-shaken-openapi.yml
  type: apiKey
- description: '"If the ''apiKey'' parameter is not specified, a pre-provisioned client IP address may be used as the backup authentication mechanism. The server first checks for availability of an ''apiKey'' in the query parameter and if it doesn''t find one, it tries to authenticate via the client IP address." (info.description, verbatim)'
  name: client-ip-allowlist
  sources:
  - openapi/transunion-trucontact-tcs-shaken-openapi.yml
  type: ip-allowlist
- description: The TruValidate Device Risk API host requires a client certificate. This is not described in any published OpenAPI — it was observed on the wire.
  evidence: GET https://api.iovation.com/ returned HTTP 403 with body "Unauthorized - missing/invalid client certificate" on 2026-08-13.
  method: probed
  name: mutual-tls
  scope: api.iovation.com (TruValidate Device Risk)
  sources:
  - probe
  type: mutualTLS
slug: transunion-authentication
source_filename: transunion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/transunion-trucontact-tcs-shaken-openapi.yml\ndocs: https://neustar.github.io/tcs-apis/\nnote: >-\n  derive-authentication.py returned zero profiles for this provider because the\n  published TruContact TCS spec declares NO components.securitySchemes at all —\n  authentication is described in prose in info.description and carried as an ordinary\n  `apiKey` QUERY parameter on all nine operations. That is the finding, and it is a\n  real weakness: a machine reading the contract cannot tell that these endpoints are\n  authenticated. Everything below is read verbatim out of the spec.\nsummary:\n  types: [apiKey, ip-allowlist, mutualTLS]\n  api_key_in: [query]\n  oauth2_flows: []\n  declared_as_security_scheme: false\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: query\n    parameter: apiKey\n    required: false\n    declared_in_spec_as: parameter\n    sources: [openapi/transunion-trucontact-tcs-shaken-openapi.yml]\n\
  \    applies_to:\n      - authn/identityj-j\n      - authn/identitys-j\n      - authn/identitys-s\n      - authn/identitymps\n      - authn/identitympj\n      - verify/identityj-j\n      - verify/identitys-j\n      - verify/identitys-s\n      - verify/identitycvt\n    description: >-\n      \"If a RESTful API client chooses to use 'apiKey' for authentication, an 'apiKey'\n      query parameter, with a pre-provisioned value, is validated to access API calls\n      that are restricted.\" (info.description, verbatim)\n  - name: client-ip-allowlist\n    type: ip-allowlist\n    sources: [openapi/transunion-trucontact-tcs-shaken-openapi.yml]\n    description: >-\n      \"If the 'apiKey' parameter is not specified, a pre-provisioned client IP address\n      may be used as the backup authentication mechanism. The server first checks for\n      availability of an 'apiKey' in the query parameter and if it doesn't find one, it\n      tries to authenticate via the client IP address.\" (info.description,\
  \ verbatim)\n  - name: mutual-tls\n    type: mutualTLS\n    sources: [probe]\n    scope: api.iovation.com (TruValidate Device Risk)\n    method: probed\n    evidence: >-\n      GET https://api.iovation.com/ returned HTTP 403 with body\n      \"Unauthorized - missing/invalid client certificate\" on 2026-08-13.\n    description: >-\n      The TruValidate Device Risk API host requires a client certificate. This is not\n      described in any published OpenAPI — it was observed on the wire.\nweaknesses:\n  - id: apikey-in-query\n    detail: >-\n      The API key travels as a URL query parameter, so it lands in proxy logs, browser\n      history and Referer headers. A header-borne key would be the RFC-friendly form.\n  - id: no-securityschemes\n    detail: >-\n      components.securitySchemes is absent and no operation carries a security[]\n      requirement, so automated clients, gateways and scanners see nine unauthenticated\n      POST endpoints. The auth model exists only in prose.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transunion/refs/heads/main/authentication/transunion-authentication.yml
summary_line: apiKey/ip-allowlist/mutualTLS · 3 schemes
tags:
- Financial
- Credit Reporting
- Risk
- Identity
- Fraud
- Marketing
- Telecommunications
- Call Authentication
- STIR/SHAKEN
---
