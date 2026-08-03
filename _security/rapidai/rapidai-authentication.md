---
api_key_in: []
auth_types:
- unknown-api-token
- saml-sso
description: ''
kind: authentication
layout: security
method: searched
name: Rapidai Authentication
name_suffix: Authentication
oauth_flows: []
overview: RapidAI secures its APIs with unknown-api-token and saml-sso across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RapidAI
provider_slug: rapidai
scheme_count: 3
schemes:
- applies_to: https://api.us.rapid-sys.com
  description: The Rapid Technology Partner API is gated. Anonymous requests to the versioned surface return HTTP 403 with an AWS API Gateway body {"message":"Missing Authentication Token"}, and unversioned paths return {"message":"Forbidden"}. The credential type is not published.
  evidence:
    fetched: '2026-08-02'
    probes:
    - body: '{"message":"Missing Authentication Token"}'
      http_status: 403
      url: https://api.us.rapid-sys.com/v4
    - body: '{"message":"Forbidden"}'
      http_status: 403
      url: https://api.us.rapid-sys.com/
    - http_status: 500
      note: An auth-discovery endpoint exists on the platform (referenced by RapidAI's own Rapid Web App bundle) but is not anonymously usable.
      url: https://api.us.rapid-sys.com/v4/auth/discovery
  name: rapid-partner-api
  type: unknown
- applies_to: https://app.rapidai.com/
  description: The Rapid Web App supports enterprise single sign-on through third-party identity providers.
  evidence:
    quote: Rapid Web App is "integrated with third-party identity providers such as Microsoft Active Directory to support single sign-on."
    source: https://www.rapidai.com/press-release/rapidai-launches-rapid-web-app-and-receives-iso-27001-certification
  name: enterprise-sso
  type: saml-sso
- applies_to: https://api.us.rapid-sys.com
  description: The Rapid mobile/web client calls a /v4/auth/device-allowed endpoint, indicating device-level authorization on top of user authentication. Not anonymously documented.
  evidence:
    source: https://app.rapidai.com/main.0aa463f11046e124.js
  name: device-authorization
  type: unknown
slug: rapidai-authentication
source_filename: rapidai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.rapidai.com/platform/workflow-integration\ndocs:\n- https://www.rapidai.com/platform/workflow-integration\n- https://www.rapidai.com/it\nnote: No OpenAPI exists for RapidAI, so nothing here was derived from securitySchemes.\n  This profile is assembled from RapidAI's own published statements plus anonymous\n  probes of the production API host. Exact token format, header name and grant type\n  are NOT public — they are disclosed to Rapid Technology Partner Program members.\nsummary:\n  types:\n  - unknown-api-token\n  - saml-sso\n  api_key_in: []\n  oauth2_flows: []\n  public_self_service: false\n  developer_portal: false\nschemes:\n- name: rapid-partner-api\n  type: unknown\n  applies_to: https://api.us.rapid-sys.com\n  description: The Rapid Technology Partner API is gated. Anonymous requests to the\n    versioned surface return HTTP 403 with an AWS API Gateway body {\"message\":\"Missing\n    Authentication Token\"\
  }, and unversioned paths return {\"message\":\"Forbidden\"}. The\n    credential type is not published.\n  evidence:\n    fetched: '2026-08-02'\n    probes:\n    - url: https://api.us.rapid-sys.com/v4\n      http_status: 403\n      body: '{\"message\":\"Missing Authentication Token\"}'\n    - url: https://api.us.rapid-sys.com/\n      http_status: 403\n      body: '{\"message\":\"Forbidden\"}'\n    - url: https://api.us.rapid-sys.com/v4/auth/discovery\n      http_status: 500\n      note: An auth-discovery endpoint exists on the platform (referenced by RapidAI's\n        own Rapid Web App bundle) but is not anonymously usable.\n- name: enterprise-sso\n  type: saml-sso\n  applies_to: https://app.rapidai.com/\n  description: The Rapid Web App supports enterprise single sign-on through third-party\n    identity providers.\n  evidence:\n    quote: 'Rapid Web App is \"integrated with third-party identity providers such as\n      Microsoft Active Directory to support single sign-on.\"'\n    source:\
  \ https://www.rapidai.com/press-release/rapidai-launches-rapid-web-app-and-receives-iso-27001-certification\n- name: device-authorization\n  type: unknown\n  applies_to: https://api.us.rapid-sys.com\n  description: The Rapid mobile/web client calls a /v4/auth/device-allowed endpoint,\n    indicating device-level authorization on top of user authentication. Not anonymously\n    documented.\n  evidence:\n    source: https://app.rapidai.com/main.0aa463f11046e124.js\ndiscovery_probes:\n- url: https://www.rapidai.com/.well-known/openid-configuration\n  http_status: 404\n- url: https://www.rapidai.com/.well-known/oauth-authorization-server\n  http_status: 404\n- url: https://api.us.rapid-sys.com/.well-known/openid-configuration\n  http_status: 403\n- url: https://api.us.rapid-sys.com/.well-known/oauth-protected-resource\n  http_status: 403\ngaps:\n- No public authentication documentation page.\n- No OAuth 2.0 / OIDC discovery document served anonymously on any host.\n- No self-service credential\
  \ issuance; access runs through the Rapid Technology Partner\n  Program (https://www.rapidai.com/partners).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidai/refs/heads/main/authentication/rapidai-authentication.yml
summary_line: unknown-api-token/saml-sso · 3 schemes
tags:
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Radiology
- Clinical Decision Support
- Stroke
- DICOM
- HL7
- FHIR
- Diagnostics
---
