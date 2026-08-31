---
api_key_in: []
auth_types: []
description: 'StorONE runs two entirely separate authentication surfaces. The S1 REST API, which manages a customer''s own storage system, uses a username/password login that mints an opaque session token carried in the Authorization header — there is no OAuth, no API-key issuance portal and no scope model, because the API is served by the customer''s controller nodes and the identity store is the system''s own user database. The Model Context Protocol endpoint on www.storone.com is the opposite: full OAuth 2.1 with PKCE, discovery metadata and a single scope.'
kind: authentication
layout: security
method: searched
name: Storone Authentication
name_suffix: Authentication
oauth_flows: []
overview: StorONE declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: StorONE
provider_slug: storone
scheme_count: 0
schemes: []
slug: storone-authentication
source_filename: storone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.onestor.com/books/rest-api/page/login\ndocs: https://docs.onestor.com/books/rest-api/page/login\nname: StorONE authentication\ndescription: >-\n  StorONE runs two entirely separate authentication surfaces. The S1 REST API, which manages a\n  customer's own storage system, uses a username/password login that mints an opaque session token\n  carried in the Authorization header — there is no OAuth, no API-key issuance portal and no scope\n  model, because the API is served by the customer's controller nodes and the identity store is the\n  system's own user database. The Model Context Protocol endpoint on www.storone.com is the opposite:\n  full OAuth 2.1 with PKCE, discovery metadata and a single scope.\nsurfaces:\n  - id: s1-rest-api\n    name: StorONE S1 REST API\n    base_url: https://{s1-controller-node}\n    docs: https://docs.onestor.com/books/rest-api/page/login\n    schemes:\n      - id: session-token\n \
  \       type: apiKey\n        in: header\n        name: Authorization\n        scheme_name_in_docs: Token\n        description: >-\n          \"API Key (Token). Parameter Name: Authorization, in: header. Authorization header token.\"\n          Every operation in the reference except POST /login and POST /resetpassword requires it.\n        obtained_by:\n          operation: POST /login\n          request_body:\n            Username: string\n            Password: string\n            TwoFactorAuthenticationToken: string\n            EmailVerficationUpdatedEmailAddress: string\n            EmailVerificationToken: string\n            InactivityTimeoutInMinutes: integer\n          response_field: SessionToken\n          success_status: 200\n          failure_status: 401\n        expiry:\n          model: inactivity timeout\n          controlled_by: InactivityTimeoutInMinutes on the login request\n          note: >-\n            The caller sets its own inactivity timeout at login. The docs\
  \ do not publish a maximum\n            or an absolute session lifetime, and there is no documented refresh operation — a client\n            re-runs POST /login.\n        header_form:\n          documented_example: 'Authorization: Bearer <token>'\n          example_in_code_samples: 'Authorization: super-extra-long-token-from-previous-output'\n          note: >-\n            The reference shows a Bearer-prefixed example under Authentication while the curl and\n            Python examples send the raw token with no scheme prefix. That inconsistency is in\n            StorONE's own docs and is recorded here rather than resolved, because it cannot be tested\n            without a live S1 system.\n    mfa:\n      supported: true\n      field: TwoFactorAuthenticationToken on POST /login\n    password_reset:\n      operation: POST /resetpassword\n      request_body:\n        Username: string\n        Email: string\n    user_management:\n      operations:\n        - POST /users/create\n     \
  \   - PUT /users/edit\n        - DELETE /users/delete\n        - GET /users/list\n      note: >-\n        Users are created and managed through the API itself, on the customer's own system. There is\n        no StorONE-hosted identity provider for this surface.\n    transport_security:\n      note: >-\n        The published Python example states the S1 system uses a self-signed certificate by default\n        and demonstrates working around it with http:// or verify=False. Credentials therefore cross\n        an unverified or plaintext channel unless the operator installs a trusted certificate. This\n        is a real, documented default and is called out because it materially affects how an agent\n        should treat this API.\n      source: https://docs.onestor.com/books/rest-api/page/python\n    oauth2: false\n    openid_connect: false\n    mutual_tls: false\n  - id: mcp-oauth\n    name: StorONE MCP server (www.storone.com)\n    base_url: https://www.storone.com/wp-json/mcp/mcp-oauth-server\n\
  \    schemes:\n      - id: oauth2-pkce\n        type: oauth2\n        flow: authorizationCode\n        pkce: S256\n        authorization_endpoint: https://www.storone.com/oauth/authorize\n        token_endpoint: https://www.storone.com/oauth/token\n        revocation_endpoint: https://www.storone.com/oauth/revoke\n        grant_types:\n          - authorization_code\n          - refresh_token\n        scopes:\n          - mcp\n        token_endpoint_auth_methods:\n          - none\n        bearer_methods:\n          - header\n        client_registration: >-\n          client_id_metadata_document_supported is true — clients identify themselves with a\n          client ID metadata document URL rather than pre-registering.\n    discovery:\n      authorization_server_metadata: https://www.storone.com/.well-known/oauth-authorization-server\n      protected_resource_metadata: https://www.storone.com/.well-known/oauth-protected-resource\n      rfc8414: true\n      rfc9728: true\n    oauth2: true\n\
  \    openid_connect: false\n    mutual_tls: false\nx-evidence:\n  - url: https://docs.onestor.com/books/rest-api/page/login\n    http_status: 200\n    fetched: '2026-08-29'\n  - url: https://docs.onestor.com/books/rest-api/page/python\n    http_status: 200\n    fetched: '2026-08-29'\n  - url: https://www.storone.com/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-29'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storone/refs/heads/main/authentication/storone-authentication.yml
summary_line: 0 schemes
tags:
- Storage
- Enterprise Storage
- Software-Defined Storage
- Data Management
- Infrastructure
- Block Storage
- File Storage
- Object Storage
- Backup
- Replication
- Snapshots
- Company
---
