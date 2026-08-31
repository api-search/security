---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: Zilla Gateway
  slug: zilla-gateway
  spec_type: Postman
  url: https://www.postman.com/aklivity-zilla/workspace/aklivity-zilla-quickstart/overview
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Aklivity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aklivity declares 9 security scheme(s) across its OpenAPI definitions.
provider_name: Aklivity
provider_slug: aklivity
scheme_count: 9
schemes:
- description: Validates a bearer JSON Web Token against a configured issuer, audience and JWKS key set. Claims are surfaced as roles usable in route guards.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/jwt.html
  edition: community
  failure_event: GUARD_JWT_AUTHORIZATION_FAILED
  id: jwt
  name: JWT guard
  note: Zilla 2.x removed the `kind` property from guard-jwt; a 1.x config that set it is now rejected rather than silently ignored. See https://docs.aklivity.io/latest/deployment/migrating-to-2.x/
  type: http-bearer
- description: Validates a shared API key presented by the client.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/api-keys.html
  edition: plus
  id: api-keys
  name: API key guard
  type: apiKey
- description: OAuth 2.0 authorization with three documented flows — client credentials for machine-to-machine, JWT bearer (RFC 7523) for asserting an existing identity, and token exchange (RFC 8693) for swapping an inbound token for a downstream one so per-user identity survives a tool call.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/oauth.html
  edition: plus
  flows:
  - docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/client-credentials/
    id: client-credentials
  - docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/jwt-bearer/
    id: jwt-bearer
  - docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/token-exchange/
    id: token-exchange
  id: oauth
  name: OAuth guard
  type: oauth2
- docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/azure-ad.html
  edition: plus
  failure_event: GUARD_AZURE_AD_AUTHORIZATION_FAILED
  id: azure-ad
  name: Azure AD guard
  type: openIdConnect
- docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-cognito.html
  edition: plus
  failure_event: GUARD_AWS_COGNITO_AUTHORIZATION_FAILED
  id: aws-cognito
  name: AWS Cognito guard
  type: openIdConnect
- docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-iam.html
  edition: plus
  id: aws-iam
  name: AWS IAM guard
  type: aws-sigv4
- description: Delegates the authorization decision to a customer-supplied Lambda function.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-lambda.html
  edition: plus
  id: aws-lambda
  name: AWS Lambda guard
  type: custom
- description: Client-certificate identity, paired with the tls binding for mTLS termination.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/x509.html
  edition: plus
  failure_event: BINDING_TLS_PEER_NOT_VERIFIED
  id: x509
  name: X.509 guard
  type: mutualTLS
- description: Credentials declared inline in zilla.yaml. Intended for development and testing, not production.
  docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/inline.html
  edition: community
  id: inline
  name: Inline guard
  type: static
slug: aklivity-authentication
source_filename: aklivity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://docs.aklivity.io/latest/reference/2.x/config/guards/\ndocs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/\nprovider: Aklivity\nproviderId: aklivity\nscope: >-\n  IMPORTANT SCOPE NOTE. Aklivity operates no hosted API, so there is no\n  Aklivity credential to obtain and no Aklivity token endpoint to call. What is\n  documented here is the authentication model Zilla ENFORCES on the API surface\n  its operator exposes — the \"guards\" a zilla.yaml attaches to routes. An agent\n  integrating with a Zilla-fronted API authenticates against the operator's own\n  identity provider, using one of the schemes below, as configured by that\n  operator. Nothing in this file is derived from an OpenAPI securityScheme,\n  because Aklivity publishes no OpenAPI of its own.\nmodel: guard-based\nplacement: >-\n  A guard is declared once under `guards:` in the namespace and referenced from\n  a route via `routes[].guarded`,\
  \ so authorization is expressed per route and\n  per binding rather than globally.\nschemes:\n  - id: jwt\n    type: http-bearer\n    name: JWT guard\n    edition: community\n    description: >-\n      Validates a bearer JSON Web Token against a configured issuer, audience\n      and JWKS key set. Claims are surfaced as roles usable in route guards.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/jwt.html\n    failure_event: GUARD_JWT_AUTHORIZATION_FAILED\n    note: >-\n      Zilla 2.x removed the `kind` property from guard-jwt; a 1.x config that\n      set it is now rejected rather than silently ignored. See\n      https://docs.aklivity.io/latest/deployment/migrating-to-2.x/\n  - id: api-keys\n    type: apiKey\n    name: API key guard\n    edition: plus\n    description: Validates a shared API key presented by the client.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/api-keys.html\n  - id: oauth\n    type: oauth2\n    name: OAuth guard\n\
  \    edition: plus\n    description: >-\n      OAuth 2.0 authorization with three documented flows — client credentials\n      for machine-to-machine, JWT bearer (RFC 7523) for asserting an existing\n      identity, and token exchange (RFC 8693) for swapping an inbound token for\n      a downstream one so per-user identity survives a tool call.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/oauth.html\n    flows:\n      - id: client-credentials\n        docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/client-credentials/\n      - id: jwt-bearer\n        docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/jwt-bearer/\n      - id: token-exchange\n        docs: https://docs.aklivity.io/latest/ai-gateway/security/oauth-guard/token-exchange/\n  - id: azure-ad\n    type: openIdConnect\n    name: Azure AD guard\n    edition: plus\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/azure-ad.html\n    failure_event:\
  \ GUARD_AZURE_AD_AUTHORIZATION_FAILED\n  - id: aws-cognito\n    type: openIdConnect\n    name: AWS Cognito guard\n    edition: plus\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-cognito.html\n    failure_event: GUARD_AWS_COGNITO_AUTHORIZATION_FAILED\n  - id: aws-iam\n    type: aws-sigv4\n    name: AWS IAM guard\n    edition: plus\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-iam.html\n  - id: aws-lambda\n    type: custom\n    name: AWS Lambda guard\n    edition: plus\n    description: Delegates the authorization decision to a customer-supplied Lambda function.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/aws-lambda.html\n  - id: x509\n    type: mutualTLS\n    name: X.509 guard\n    edition: plus\n    description: Client-certificate identity, paired with the tls binding for mTLS termination.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/x509.html\n    failure_event: BINDING_TLS_PEER_NOT_VERIFIED\n\
  \  - id: inline\n    type: static\n    name: Inline guard\n    edition: community\n    description: Credentials declared inline in zilla.yaml. Intended for development and testing, not production.\n    docs: https://docs.aklivity.io/latest/reference/2.x/config/guards/inline.html\ntransport_security:\n  - id: tls\n    description: TLS termination and origination, with SNI-based routing.\n    docs: https://docs.aklivity.io/latest/ai-gateway/security/tls/\n  - id: mtls\n    description: Mutual TLS between agent/client and gateway, and between gateway and upstream.\n    docs: https://docs.aklivity.io/latest/ai-gateway/security/tls/mtls/\nupstream_credentials:\n  description: >-\n    Credentials Zilla itself presents to a backend, rather than credentials it\n    checks.\n  kafka_sasl:\n    mechanisms:\n      - PLAIN\n      - SCRAM\n    note: >-\n      Zilla 2.x replaced `binding-kafka options.sasl` with\n      `options.authorization`. Events BINDING_KAFKA_AUTHORIZATION_FAILED and\n      BINDING_KAFKA_CLUSTER_AUTHORIZATION_FAILED\
  \ report failures.\n  vaults:\n    - id: filesystem\n      docs: https://docs.aklivity.io/latest/reference/2.x/config/vaults/filesystem.html\n    - id: aws-secrets\n      description: AWS Secrets Manager. Plus/Enterprise.\n      failure_event: VAULT_AWS_SECRETS_KEY_PAIR_INVALID\nself_service:\n  description: >-\n    The Zilla Console (Enterprise, or a flat-rate add-on to Plus) adds a\n    self-service developer portal where a consumer subscribes to an API Product\n    and is issued an API key or client certificate under that product's plan.\n    The Console is deployed by the customer via Helm; there is no Aklivity-hosted\n    portal to sign up for.\n  docs: https://docs.aklivity.io/latest/zilla-console/api-catalog/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aklivity/refs/heads/main/authentication/aklivity-authentication.yml
summary_line: 9 schemes
tags:
- AI Gateway
- API Gateway
- Agent Infrastructure
- Apache Kafka
- AsyncAPI
- Event-Driven
- IoT
- Kafka Proxy
- MCP
- Multi-Protocol
- Open-Source
- Real-Time
---
