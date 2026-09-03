---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Trisotech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trisotech declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Trisotech
provider_slug: trisotech
scheme_count: 0
schemes: []
slug: trisotech-authentication
source_filename: trisotech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://cloud.trisotech.com/help/des/system-integration/rest-api.html\ndocs:\n  - https://cloud.trisotech.com/help/des/system-integration/rest-api.html\n  - https://cloud.trisotech.com/help/admin/client-apps.html\n  - https://cloud.trisotech.com/help/des/system-integration/rest-api-documentation.html\nname: Trisotech Digital Enterprise Suite Authentication\nsummary: >-\n  The Trisotech Public API is protected with OAuth 2. Every call carries a bearer token in\n  the Authorization header; tokens are issued to a Client App created in the Digital\n  Enterprise Suite Administration application, and the app's granted scopes bound the token.\n  End-user sign-in to the suite itself federates through SAML2 or OpenID Connect.\nsecuritySchemes:\n  - key: oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://{instance}.trisotech.com/oauth2/auth\n    tokenUrl: https://{instance}.trisotech.com/oauth2/token\n\
  \    pkce: supported\n    description: >-\n      Standard OAuth 2 authorization code flow (standard or PKCE) requiring a user\n      authorization. This is the primary flow the provider documents.\n    scopes_ref: scopes/trisotech-scopes.yml\n  - key: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://{instance}.trisotech.com/oauth2/token\n    description: >-\n      System-to-system flow, enabled per Client App with the \"Support Client Credentials\"\n      flag. The app's Associated System Account is the identity used for access checks.\n    caveat: >-\n      The Client Apps admin page states the suite \"does not currently support apps\n      authorization (eg. Client Credentials flow) and require an access code flow\", while\n      the same page documents a \"Support Client Credentials\" toggle and an associated\n      system account. Both statements are the provider's own; treat client_credentials as\n      available but instance/version\
  \ dependent and confirm against your own instance.\n    scopes_ref: scopes/trisotech-scopes.yml\n  - key: bearer\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    description: >-\n      \"Authorization: Bearer <token>\". A bearer token can also be generated manually from\n      the Administration application with a chosen expiry. The provider states a bearer\n      token \"should be kept secret and is the equivalent of a username/password combination.\"\nidentity_federation:\n  user_login:\n    - SAML 2.0\n    - OpenID Connect (OIDC)\n  provisioning:\n    - standard: SCIM\n      docs: https://cloud.trisotech.com/help/admin/scim-aad.html\n      note: SCIM user/group provisioning is documented for Azure AD / Entra ID.\n  source: https://www.trisotech.com/security/\nrequest_requirements:\n  - header: Authorization\n    value: Bearer <token>\n    required: true\n    exception: the Public API Login resource\n  - header: Accept\n    value: application/json\n\
  \    required: recommended\n    note: >-\n      \"By default, if the Accept header is not defined, the API produces XML results for\n      legacy support. This format is deprecated.\" Always send Accept: application/json.\nunauthenticated_behaviour:\n  probed: '2026-09-02'\n  request: GET https://cloud.trisotech.com/publicapi/user (no Authorization header)\n  http_status: 500\n  body: '{\"error\":[{\"code\":\"RequiresLogin\",\"systemMessage\":\"This service requires a User Login\",\"userMessage\":\"You should Login First\"}]}'\n  finding: >-\n    Missing credentials are answered with HTTP 500 and an application error code, not the\n    RFC 7235 401 an agent expects. An automated client cannot distinguish \"not authenticated\"\n    from \"server fault\" by status code alone and must read error[].code.\napi_key: null\nmutual_tls: null\nevidence:\n  - url: https://cloud.trisotech.com/help/des/system-integration/rest-api.html\n    status: 200\n  - url: https://cloud.trisotech.com/help/admin/client-apps.html\n\
  \    status: 200\n  - url: https://cloud.trisotech.com/publicapi/user\n    status: 500\n  - url: https://cloud.trisotech.com/publicapi/login\n    status: 200\n  - url: https://cloud.trisotech.com/oauth2/auth\n    status: 200\n    note: redirects to the instance login when unauthenticated\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trisotech/refs/heads/main/authentication/trisotech-authentication.yml
summary_line: 0 schemes
tags:
- Business Process Management
- Decision Management
- Workflow Automation
- Low Code
- BPMN
- DMN
- CMMN
- Healthcare
- FHIR
- Clinical Decision Support
- Standards
- AI Agents
- Model Context Protocol
- Enterprise Architecture
---
