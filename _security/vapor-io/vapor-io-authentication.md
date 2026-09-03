---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Vapor Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vapor IO declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Vapor IO
provider_slug: vapor-io
scheme_count: 0
schemes: []
slug: vapor-io-authentication
source_filename: vapor-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://synse.readthedocs.io/en/latest/server/user/advanced/#secure-communication and /server/user/configuration/\nprovider: Vapor IO\napi: Synse Server API (v3)\nsummary: 'Synse Server publishes NO application-level authentication or authorization. The platform overview\n  states this outright under ''What Synse Does Not Provide'': ''Access control to plugins/devices.'' Every\n  documented HTTP and WebSocket operation, including the two write operations that act on physical hardware,\n  is unauthenticated. Security is transport-level and is the operator''s responsibility.'\nsecurity_schemes: []\nauth_required: false\ntransport_security:\n- name: server TLS\n  description: The HTTP/WebSocket API can be served over TLS by supplying a certificate and key.\n  config:\n    yaml_keys:\n    - ssl.cert\n    - ssl.key\n    env:\n    - SYNSE_SSL_CERT\n    - SYNSE_SSL_KEY\n  docs: https://synse.readthedocs.io/en/latest/server/user/configuration/#ssl\n\
  \  note: 'The docs recommend a TLS-terminating frontend such as Nginx for production rather than the built-in\n    option: ''While this may work for small/personal use cases, it is recommended to use a more robust\n    TLS termination frontend for it in production.'''\n- name: plugin gRPC TLS\n  description: The internal Synse Server to plugin gRPC channel can be secured with TLS.\n  config:\n    yaml_keys:\n    - grpc.tls.cert\n    env:\n    - SYNSE_GRPC_TLS_CERT\n  docs: https://synse.readthedocs.io/en/latest/server/user/configuration/#tls\n  note: Synse performs no certificate generation or management; the operator supplies and rotates certs.\noauth2: false\noidc: false\napi_keys: false\nmtls: false\nagent_guidance: An agent calling a Synse deployment needs no credential and will not be told it lacks\n  authority. The only thing standing between a caller and a write to physical hardware is network reach,\n  so treat network placement, not an auth header, as the access control boundary.\n\
  docs: https://synse.readthedocs.io/en/latest/server/user/advanced/#secure-communication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapor-io/refs/heads/main/authentication/vapor-io-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Edge Computing
- Data Centers
- Colocation
- Infrastructure
- Device Management
- Monitoring
- Telemetry
- IoT
- gRPC
- Open Source
- Kubernetes
---
