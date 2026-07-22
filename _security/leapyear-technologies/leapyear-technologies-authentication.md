---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Leapyear Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeapYear Technologies declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LeapYear Technologies
provider_slug: leapyear-technologies
scheme_count: 2
schemes:
- client: leapyear.Client
  description: Username and password passed directly to the client constructor, which establishes an authenticated session against a customer-operated server.
  id: client-credentials
  parameters:
  - description: LeapYear Core server endpoint, e.g. 'http://localhost:4401'. Port is commonly supplied via the LY_PORT environment variable.
    name: url
  - description: User account identifier.
    name: username
  - description: User account password.
    name: password
  scheme: basic-equivalent
  session:
    connection_check: client.connected
    context_manager: 'with Client(url, username, password) as client:'
    evidence: leapyear.exceptions.TokenExpiredError ("Authentication token was expired") indicates the client holds a server-issued session token after the initial credential exchange.
    token_based: true
  signature: Client(url, username, password)
  type: http
- description: Public key authentication credentials are supported; referenced by the PublicKeyCredentialsError exception class in leapyear.exceptions.
  detail: The published reference confirms the credential type exists but does not document the enrollment or key-format procedure publicly.
  evidence: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/exceptions.html
  id: public-key
  type: publicKey
slug: leapyear-technologies-authentication
source_filename: leapyear-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/tutorial.html\ndocs: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/tutorial.html\nnotes: >-\n  LeapYear Core was licensed, self-hosted enterprise software, not a public\n  multi-tenant API — there is no public authorization server, no OAuth surface,\n  and no signup. Authentication is against the customer's own LeapYear server\n  instance via the `leapyear` Python client. Captured from the published 4.1.1\n  documentation, which remains live after the Snowflake acquisition.\ndeployment: self-hosted\noauth2: false\nopenid_connect: false\napi_keys: false\nschemes:\n  - id: client-credentials\n    type: http\n    scheme: basic-equivalent\n    description: >-\n      Username and password passed directly to the client constructor, which\n      establishes an authenticated session against a customer-operated server.\n    client: leapyear.Client\n    signature:\
  \ Client(url, username, password)\n    parameters:\n      - name: url\n        description: >-\n          LeapYear Core server endpoint, e.g. 'http://localhost:4401'. Port is\n          commonly supplied via the LY_PORT environment variable.\n      - name: username\n        description: User account identifier.\n      - name: password\n        description: User account password.\n    session:\n      token_based: true\n      evidence: >-\n        leapyear.exceptions.TokenExpiredError (\"Authentication token was\n        expired\") indicates the client holds a server-issued session token\n        after the initial credential exchange.\n      connection_check: client.connected\n      context_manager: 'with Client(url, username, password) as client:'\n  - id: public-key\n    type: publicKey\n    description: >-\n      Public key authentication credentials are supported; referenced by the\n      PublicKeyCredentialsError exception class in leapyear.exceptions.\n    evidence: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/exceptions.html\n\
  \    detail: >-\n      The published reference confirms the credential type exists but does not\n      document the enrollment or key-format procedure publicly.\ntransport_security:\n  tls: supported\n  evidence: leapyear.exceptions.TLSError (\"Errors from TLS.\")\nenvironment_variables:\n  - name: LY_PORT\n    description: Server port used to construct the client URL; documented default 4401.\nauthorization_model:\n  scopes: false\n  description: >-\n    Authorization is grant-based rather than scope-based, administered\n    server-side through the leapyear.admin.grants module over Database, Table,\n    View and User objects — plus a per-user differential-privacy exposure\n    budget that acts as a second, quantitative authorization limit.\n  reference: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/admin_grants.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapyear-technologies/refs/heads/main/authentication/leapyear-technologies-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Ai Infrastructure
- Differential Privacy
- Data Privacy
- Machine Learning
- Data Clean Rooms
- Privacy Enhancing Technologies
- Acquired
---
