---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sibel Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sibel Health declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Sibel Health
provider_slug: sibel-health
scheme_count: 3
schemes:
- confidence: medium
  evidence: Authorization is named in the Access-Control-Allow-Headers list the gateway returns, so the API accepts a bearer/signed credential in that header. The token format is not disclosed anonymously and is not documented publicly.
  id: authorization-header
  location: header
  name: Authorization
  status: advertised
  type: http
- confidence: medium
  evidence: X-Api-Key is named in the Access-Control-Allow-Headers list. This is the AWS API Gateway usage-plan API key header; its presence indicates a key-based access tier, but no key issuance, rotation, or scope documentation is published.
  id: api-key-header
  location: header
  name: X-Api-Key
  status: advertised
  type: apiKey
- confidence: low
  evidence: X-Amz-Date and X-Amz-Security-Token appear in the allowed-headers list, which is consistent with AWS SigV4 / IAM authorization, but this is also the AWS API Gateway default CORS header set and therefore weak evidence on its own. Not asserted as the live scheme.
  id: aws-sigv4
  location: header
  name: X-Amz-Date / X-Amz-Security-Token
  status: possible
  type: http
slug: sibel-health-authentication
source_filename: sibel-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: 'anonymous HTTP probes of https://api.sibelhealth.com/jsn/alpha (2026-08-27); base URL read\n  from the JavaScript bundle of Sibel Health''s own datahub.sibelhealth.com single-page application'\napi: Sibel Health ANNE Cloud API\nsummary: 'Sibel Health publishes no authentication documentation. Everything below was observed\n  directly on the wire against the live API host. There is no OpenAPI securitySchemes block to\n  derive from, so nothing here is derived — it is only what the server itself disclosed.'\nobserved:\n  gateway: AWS API Gateway\n  gateway_evidence:\n  - 'response header x-amzn-errortype: MissingAuthenticationTokenException'\n  - response headers x-amz-apigw-id and x-amzn-requestid present on every response\n  anonymous_response:\n    status: 403\n    bodies:\n    - '{\"message\":\"Forbidden\"}'\n    - '{\"message\":\"Missing Authentication Token\"}'\n    content_type: application/json\n  cors:\n    access_control_allow_origin:\
  \ '*'\n    access_control_allow_methods: DELETE,GET,HEAD,OPTIONS,PATCH,POST,PUT\n    access_control_allow_headers: Content-Type,X-Amz-Date,Authorization,X-Api-Key,X-Amz-Security-Token\nschemes:\n- id: authorization-header\n  type: http\n  location: header\n  name: Authorization\n  status: advertised\n  confidence: medium\n  evidence: 'Authorization is named in the Access-Control-Allow-Headers list the gateway returns,\n    so the API accepts a bearer/signed credential in that header. The token format is not disclosed\n    anonymously and is not documented publicly.'\n- id: api-key-header\n  type: apiKey\n  location: header\n  name: X-Api-Key\n  status: advertised\n  confidence: medium\n  evidence: 'X-Api-Key is named in the Access-Control-Allow-Headers list. This is the AWS API Gateway\n    usage-plan API key header; its presence indicates a key-based access tier, but no key issuance,\n    rotation, or scope documentation is published.'\n- id: aws-sigv4\n  type: http\n  location: header\n\
  \  name: X-Amz-Date / X-Amz-Security-Token\n  status: possible\n  confidence: low\n  evidence: 'X-Amz-Date and X-Amz-Security-Token appear in the allowed-headers list, which is\n    consistent with AWS SigV4 / IAM authorization, but this is also the AWS API Gateway default CORS\n    header set and therefore weak evidence on its own. Not asserted as the live scheme.'\noauth:\n  documented: false\n  discovery_probed: true\n  note: '/.well-known/openid-configuration and /.well-known/oauth-authorization-server were probed on\n    both sibelhealth.com (404) and api.sibelhealth.com (403). No OAuth or OIDC discovery document is\n    served, so scopes/ is not applicable and no scopes artifact is written.'\ndocs:\n  developer_portal: null\n  auth_documentation_url: null\n  note: 'developer.sibelhealth.com holds a valid TLS certificate (present in Certificate Transparency\n    logs) and resolves to 76.29.17.158, but does not answer HTTP — no response within a 12s deadline\n    on 2026-08-27. No\
  \ other public documentation host was found.'\nevidence:\n- url: https://api.sibelhealth.com/jsn/alpha\n  status: 403\n- url: https://api.sibelhealth.com/\n  status: 403\n- url: https://developer.sibelhealth.com/\n  status: <no response>\n- url: https://sibelhealth.com/.well-known/openid-configuration\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sibel-health/refs/heads/main/authentication/sibel-health-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Remote Patient Monitoring
- Wearables
- Digital Health
- Vital Signs
- Clinical Trials
- Sensors
- Internet of Things
- Sleep
---
