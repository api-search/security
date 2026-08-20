---
api_key_in:
- cookie
api_specs:
- filename: intersight-fabric-openapi.json
  format: json
  label: Cisco Intersight Fabric API
  slug: fabric
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-fabric-openapi.json
- filename: intersight-hyperflex-openapi.json
  format: json
  label: Cisco Intersight HyperFlex API
  slug: hyperflex
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-hyperflex-openapi.json
- filename: intersight-kubernetes-openapi.json
  format: json
  label: Cisco Intersight Kubernetes API
  slug: kubernetes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-kubernetes-openapi.json
- filename: intersight-nexus-insight-advisor-openapi.json
  format: json
  label: Cisco Intersight Nexus Insight Advisor API
  slug: nexus-insight-advisor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-nexus-insight-advisor-openapi.json
- filename: intersight-orchestrator-openapi.json
  format: json
  label: Cisco Intersight Orchestrator API
  slug: orchestrator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-orchestrator-openapi.json
- filename: intersight-server-openapi.json
  format: json
  label: Cisco Intersight Server API
  slug: server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-server-openapi.json
- filename: intersight-storage-openapi.json
  format: json
  label: Cisco Intersight Storage API
  slug: storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-storage-openapi.json
- filename: intersight-system-openapi.json
  format: json
  label: Cisco Intersight System API
  slug: system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-system-openapi.json
- filename: intersight-telemetry-openapi.json
  format: json
  label: Cisco Intersight Telemetry API
  slug: telemetry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-telemetry-openapi.json
- filename: intersight-virtualization-openapi.json
  format: json
  label: Cisco Intersight Virtualization API
  slug: virtualization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-virtualization-openapi.json
- filename: intersight-workflows-openapi.json
  format: json
  label: Cisco Intersight Workflows API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/openapi/intersight-workflows-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Intersight Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cisco Intersight secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cisco Intersight
provider_slug: intersight
scheme_count: 3
schemes:
- description: The authentication cookie obtained from a Single-Sign-On SAML assertion.
  in: cookie
  name: cookieAuth
  parameter: X-Starship-Token
  sources:
  - openapi/intersight-fabric-openapi.json
  - openapi/intersight-hyperflex-openapi.json
  - openapi/intersight-kubernetes-openapi.json
  - openapi/intersight-nexus-insight-advisor-openapi.json
  - openapi/intersight-orchestrator-openapi.json
  - openapi/intersight-server-openapi.json
  - openapi/intersight-storage-openapi.json
  - openapi/intersight-system-openapi.json
  - openapi/intersight-telemetry-openapi.json
  - openapi/intersight-virtualization-openapi.json
  - openapi/intersight-workflows-openapi.json
  type: apiKey
- description: "The 'HTTP signature' security scheme. Each HTTP request is cryptographically signed\nas specified in https://datatracker.ietf.org/doc/draft-cavage-http-signatures/.\nSee [Intersight API and SDK documentation](https://intersight.com/apidocs) for details\nabout how to configure the HTTP signature scheme.\nYou must include the following fields in the signed headers.\n  1. '(request-target)'\n  1. '(created"
  name: http_signature
  scheme: signature
  sources:
  - openapi/intersight-fabric-openapi.json
  - openapi/intersight-hyperflex-openapi.json
  - openapi/intersight-kubernetes-openapi.json
  - openapi/intersight-nexus-insight-advisor-openapi.json
  - openapi/intersight-orchestrator-openapi.json
  - openapi/intersight-server-openapi.json
  - openapi/intersight-storage-openapi.json
  - openapi/intersight-system-openapi.json
  - openapi/intersight-telemetry-openapi.json
  - openapi/intersight-virtualization-openapi.json
  - openapi/intersight-workflows-openapi.json
  type: http
- description: 'The client uses the OAuth2 security scheme. To use OAuth2, a client application

    must be registered by creating a iam.AppRegistration resource.

    The user who creates the iam.AppRegistration resource can specify a list of OAuth2

    scopes. These iam.AppRegistration scopes restricts which subset of scopes

    a registered client can obtain.

    Supported OAuth2 flows are:

    **Authorization Code**

    In the authorizat'
  flows:
  - authorizationUrl: /iam/app-authorize
    flow: authorizationCode
    scopes: 54
    tokenUrl: /iam/token
  - flow: clientCredentials
    scopes: 3315
    tokenUrl: /iam/token
  name: oAuth2
  sources:
  - openapi/intersight-fabric-openapi.json
  - openapi/intersight-hyperflex-openapi.json
  - openapi/intersight-kubernetes-openapi.json
  - openapi/intersight-nexus-insight-advisor-openapi.json
  - openapi/intersight-orchestrator-openapi.json
  - openapi/intersight-server-openapi.json
  - openapi/intersight-storage-openapi.json
  - openapi/intersight-system-openapi.json
  - openapi/intersight-telemetry-openapi.json
  - openapi/intersight-virtualization-openapi.json
  - openapi/intersight-workflows-openapi.json
  type: oauth2
slug: intersight-authentication
source_filename: intersight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/intersight-fabric-openapi.json, openapi/intersight-hyperflex-openapi.json, openapi/intersight-kubernetes-openapi.json,\n  openapi/intersight-nexus-insight-advisor-openapi.json, openapi/intersight-orchestrator-openapi.json,\n  openapi/intersight-server-openapi.json, openapi/intersight-storage-openapi.json, openapi/intersight-system-openapi.json,\n  openapi/intersight-telemetry-openapi.json, openapi/intersight-virtualization-openapi.json,\n  openapi/intersight-workflows-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: X-Starship-Token\n  description: The authentication cookie obtained from a Single-Sign-On SAML assertion.\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n\
  \  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- name: http_signature\n  type: http\n  scheme: signature\n  description: |-\n    The 'HTTP signature' security scheme. Each HTTP request is cryptographically signed\n    as specified in https://datatracker.ietf.org/doc/draft-cavage-http-signatures/.\n    See [Intersight API and SDK documentation](https://intersight.com/apidocs) for details\n    about how to configure the HTTP signature scheme.\n    You must include the following fields in the signed headers.\n      1. '(request-target)'\n      1. '(created\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n\
  \  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /iam/app-authorize\n    tokenUrl: /iam/token\n    scopes: 54\n  - flow: clientCredentials\n    tokenUrl: /iam/token\n    scopes: 3315\n  description: |-\n    The client uses the OAuth2 security scheme. To use OAuth2, a client application\n    must be registered by creating a iam.AppRegistration resource.\n    The user who creates the iam.AppRegistration resource can specify a list of OAuth2\n    scopes. These iam.AppRegistration scopes restricts which subset of scopes\n\
  \    a registered client can obtain.\n    Supported OAuth2 flows are:\n    **Authorization Code**\n    In the authorizat\n  sources:\n  - openapi/intersight-fabric-openapi.json\n  - openapi/intersight-hyperflex-openapi.json\n  - openapi/intersight-kubernetes-openapi.json\n  - openapi/intersight-nexus-insight-advisor-openapi.json\n  - openapi/intersight-orchestrator-openapi.json\n  - openapi/intersight-server-openapi.json\n  - openapi/intersight-storage-openapi.json\n  - openapi/intersight-system-openapi.json\n  - openapi/intersight-telemetry-openapi.json\n  - openapi/intersight-virtualization-openapi.json\n  - openapi/intersight-workflows-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intersight/refs/heads/main/authentication/intersight-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Infrastructure
- Cloud Operations
- Data-Center
- Compute
- Networking
- Enterprise
- Storage
- Virtualization
- Kubernetes
- Orchestration
- Telemetry
- Firmware Management
---
