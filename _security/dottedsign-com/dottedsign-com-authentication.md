---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dottedsign-com-download-api-openapi.yml
  format: yaml
  label: DottedSign Download API
  slug: dottedsign-com-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-download-api-openapi.yml
- filename: dottedsign-com-general-api-openapi.yml
  format: yaml
  label: DottedSign General API
  slug: dottedsign-com-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-general-api-openapi.yml
- filename: dottedsign-com-management-api-openapi.yml
  format: yaml
  label: DottedSign Management API
  slug: dottedsign-com-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-management-api-openapi.yml
- filename: dottedsign-com-seal-api-openapi.yml
  format: yaml
  label: DottedSign Seal API
  slug: dottedsign-com-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-seal-api-openapi.yml
- filename: dottedsign-com-signature-api-openapi.yml
  format: yaml
  label: DottedSign Signature API
  slug: dottedsign-com-signature-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signature-api-openapi.yml
- filename: dottedsign-com-signing-api-openapi.yml
  format: yaml
  label: DottedSign Signing API
  slug: dottedsign-com-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signing-api-openapi.yml
- filename: dottedsign-com-signtask-api-openapi.yml
  format: yaml
  label: DottedSign Sign Task API
  slug: dottedsign-com-signtask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signtask-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: DottedSign Authentication
name_suffix: Authentication
oauth_flows: []
overview: DottedSign declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: DottedSign
provider_slug: dottedsign-com
scheme_count: 3
schemes:
- evidence: The **Client Credentials Flow** involves an application exchanging its credentials, such as the client ID and client secret, for an access token.
  flows:
  - client_credentials
  how_to_obtain: Obtain a client ID and client secret from the DottedSign application settings.
  name: client_credentials
  token_url: /v1/oauth/token
  type: oauth2
- authorize_url: /v1/oauth/authorize
  evidence: The **Authorization Code Flow** involves an application directing the user to an authentication page where they can log in and authorize the application.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register a redirect URL in your application and use the client ID and client secret to request an authorization code.
  name: authorization_code
  token_url: /v1/oauth/token
  type: oauth2
- authorize_url: /v1/oauth/authorize
  evidence: The **JWT Authorization Grant Flow** is an authorization mechanism where the application directs users to an authentication page for login and authorization.
  flows:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - refresh_token
  how_to_obtain: Generate a JWT assertion using the application’s secret and include it with the client ID and client secret.
  name: jwt_bearer
  token_url: /v1/oauth/token
  type: oauth2
slug: dottedsign-com-authentication
source_filename: dottedsign-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.dottedsign.com/docs/02-authentication-01-client-credentials-flow.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.dottedsign.com/docs/02-authentication-01-client-credentials-flow.md\nsources:\n- https://developer.dottedsign.com/docs/02-authentication-01-client-credentials-flow.md\n- https://developer.dottedsign.com/docs/02-authentication-02-authorization-code-flow.md\n- https://developer.dottedsign.com/docs/02-authentication-03-jwt-authorization-grant-flow.md\n- https://developer.dottedsign.com/docs/02-authentication-01-client-credentials-flow\nschemes:\n- type: oauth2\n  name: client_credentials\n  evidence: The **Client Credentials Flow** involves an application exchanging its credentials, such as the client ID and client secret, for an\n    access token.\n  flows:\n  - client_credentials\n  token_url: /v1/oauth/token\n  how_to_obtain: Obtain a client ID and client secret from the DottedSign application settings.\n- type: oauth2\n  name: authorization_code\n  evidence: The\
  \ **Authorization Code Flow** involves an application directing the user to an authentication page where they can log in and authorize\n    the application.\n  flows:\n  - authorization_code\n  - refresh_token\n  token_url: /v1/oauth/token\n  authorize_url: /v1/oauth/authorize\n  how_to_obtain: Register a redirect URL in your application and use the client ID and client secret to request an authorization code.\n- type: oauth2\n  name: jwt_bearer\n  evidence: The **JWT Authorization Grant Flow** is an authorization mechanism where the application directs users to an authentication page for\n    login and authorization.\n  flows:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - refresh_token\n  token_url: /v1/oauth/token\n  authorize_url: /v1/oauth/authorize\n  how_to_obtain: Generate a JWT assertion using the application’s secret and include it with the client ID and client secret.\ndocs: https://developer.dottedsign.com/docs/02-authentication-01-client-credentials-flow.md\n"
source_yaml_url: https://artifacts.apis.io/dottedsign-com/authentication/dottedsign-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- E-Signature
- Workflows
- Software-as-a-Service
- Document Management
---
