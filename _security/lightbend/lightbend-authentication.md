---
api_key_in: []
auth_types:
- interactive-login
- token
- jwt
- mtls
- acl
description: ''
kind: authentication
layout: security
method: searched
name: Lightbend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightbend secures its APIs with interactive-login, token, jwt, mtls, and acl across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightbend
provider_slug: lightbend
scheme_count: 0
schemes: []
slug: lightbend-authentication
source_filename: lightbend-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.akka.io/reference/cli/akka-cli/index.html
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsources:\n  - https://doc.akka.io/reference/cli/akka-cli/index.html\n  - https://doc.akka.io/sdk/integrations/identity-and-security.html\n  - https://doc.akka.io/operations/projects/secrets.html\ndocs: https://doc.akka.io/sdk/integrations/identity-and-security.html\nnotes: >-\n  Lightbend (dba Akka) publishes no public OpenAPI for its control plane, so this profile is captured from the CLI\n  reference and the SDK identity/security documentation rather than derived from securitySchemes. Two distinct\n  surfaces exist: platform/control-plane authentication (how you authenticate the CLI and CI against Akka), and\n  service authentication (how the services you build on Akka authenticate their own callers).\nsummary:\n  types: [interactive-login, token, jwt, mtls, acl]\n  api_key_in: []\n  oauth2_flows: []\nplatform_auth:\n  description: Authenticating the Akka CLI, CI/CD and the console against the Akka platform.\n  mechanisms:\n    -\
  \ name: Interactive login\n      command: akka auth login\n      description: Browser-based interactive login binding the CLI to a user account.\n    - name: Service / project tokens\n      command: akka auth tokens\n      related: [akka auth use-token, akka projects tokens]\n      description: Long-lived tokens for non-interactive use in CI/CD pipelines.\n    - name: Container registry credentials\n      command: akka auth container-registry\n      related: [akka docker add-credentials]\n      description: Credentials for the Akka container registry and external registries.\n    - name: SDK download token\n      command: akka code token\n      description: Token configured during dev-env setup to resolve Akka SDK dependencies.\n  contexts:\n    file: ~/.akka/config.yaml\n    commands: [akka config use-context, akka config current-context]\n  console: https://console.akka.io/login\nservice_auth:\n  description: Authenticating callers of the services a developer builds and deploys on Akka.\n\
  \  mechanisms:\n    - name: ACLs\n      annotation: \"@Acl\"\n      description: Declarative access control on HTTP, gRPC and MCP endpoints, scoped by principal (e.g. Acl.Principal.ALL, internet, service).\n    - name: JWT / JWKS\n      commands: [akka services jwts, akka services jwks]\n      description: Per-service JWT validation configuration and JWKS key set management.\n    - name: TLS certificates\n      docs: https://doc.akka.io/operations/tls-certificates.html\n      description: Configuring and managing TLS certificates, including client certificate validation on exposed routes.\n    - name: Secrets\n      docs: https://doc.akka.io/operations/projects/secrets.html\n      commands: [akka secrets create, akka secrets external]\n      description: Built-in secret storage with Azure Key Vault integration for externally managed secrets.\nauthorization:\n  model: role-bindings\n  commands: [akka roles list, akka roles add-binding, akka roles delete-binding, akka roles invitations]\n\
  \  scoped_to: [organization, project]\noauth2: false\noauth_scopes: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightbend/refs/heads/main/authentication/lightbend-authentication.yml
summary_line: interactive-login/token/jwt/mtls/acl · 0 schemes
tags:
- Company
- Ai Infrastructure
- Agentic Ai
- Actor Model
- Distributed Systems
- Reactive
- Java
- Scala
- Orchestration
- Ai Governance
---
