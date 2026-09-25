---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hami-robots-txt-api-openapi.yml
  format: yaml
  label: HAMi Robots.txt API
  slug: hami-robots-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/openapi/hami-robots-txt-api-openapi.yml
- filename: hami-well-known-api-openapi.yml
  format: yaml
  label: HAMi .well Known API
  slug: hami-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/openapi/hami-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Hami Authentication
name_suffix: Authentication
oauth_flows: []
overview: HAMi declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: HAMi
provider_slug: hami
scheme_count: 0
schemes: []
slug: hami-authentication
source_filename: hami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  grpc/hami-webui-*.proto, https://github.com/Project-HAMi/HAMi-WebUI/blob/main/charts/hami-webui/values.yaml,\n  https://github.com/Project-HAMi/HAMi-WebUI/blob/main/server/internal/conf/conf.proto,\n  https://project-hami.io/docs/installation/webui-installation,\n  https://project-hami.io/.well-known/oauth-protected-resource,\n  openapi/hami-website-discovery-openapi.json\ndocs: https://project-hami.io/docs/installation/webui-installation\nnote: >-\n  Neither published HAMi API surface authenticates its callers, and that is a finding rather than a gap\n  in our research. The HAMi WebUI contract declares no security scheme in any of its five .proto files\n  and no auth interceptor is configured in the shipped server config; the documented access pattern is\n  `kubectl port-forward service/my-hami-webui 3000:3000` with the docs stating plainly that \"HAMi WebUI\n  is exposed via localhost only\". Access control is therefore\
  \ delegated entirely to Kubernetes — RBAC\n  on the port-forward, network policy, and whatever the operator puts in front of the optional Ingress.\n  The `authorization` and `basicAuth` settings in the Helm values are OUTBOUND credentials the WebUI\n  uses when scraping the operator's Prometheus, not inbound API authentication; conf.proto places both\n  inside the `Prometheus` message, and the older flat `auth` field there is marked deprecated. The\n  website discovery API is anonymous static content and says so: its own\n  /.well-known/oauth-protected-resource returns an empty authorization_servers[] and scopes_supported[].\nsecurity_schemes: []\nsurfaces:\n  - api: HAMi WebUI API\n    authentication: none\n    model: network-scoped\n    enforcement: >-\n      Kubernetes RBAC on `kubectl port-forward`, cluster network policy, and any authenticating proxy\n      the operator places in front of the optional Ingress. Nothing in the shipped artifact\n      authenticates a request that reaches\
  \ the backend.\n    transport: >-\n      HTTP on 0.0.0.0:8000 and gRPC on 0.0.0.0:9000 inside the pod; the Helm service publishes port\n      3000. TLS is not terminated by the application.\n    evidence:\n      - https://github.com/Project-HAMi/HAMi-WebUI/blob/main/server/config/config.yaml\n      - https://project-hami.io/docs/installation/webui-installation\n  - api: HAMi Website Discovery API\n    authentication: none\n    model: public\n    enforcement: Public static documents served over TLS 1.3 by Netlify with HSTS max-age 31536000.\n    evidence:\n      - https://project-hami.io/.well-known/oauth-protected-resource\n      - openapi/hami-website-discovery-openapi.json\noutbound_credentials:\n  - name: Prometheus authorization\n    where: Helm values `externalPrometheus`/`prometheus.authorization` -> conf.proto Prometheus.authorization\n    type: HTTP Authorization header credential mounted from a Kubernetes Secret\n    direction: outbound (WebUI -> operator's Prometheus)\n  - name:\
  \ Prometheus basic auth\n    where: Helm values `prometheus.basicAuth` -> conf.proto Prometheus.basic_auth\n    type: username/password mounted from a Kubernetes Secret, mutually exclusive with authorization\n    direction: outbound (WebUI -> operator's Prometheus)\n  - name: Prometheus TLS trust material\n    where: conf.proto Prometheus.tls\n    type: CA / client certificate mounted from a Kubernetes Secret\n    direction: outbound (WebUI -> operator's Prometheus)\ndeprecated:\n  - field: Prometheus.auth\n    note: Marked `[deprecated = true]` in conf.proto — \"use authorization or basic_auth with credentials mounted from files\".\noauth: false\noidc: false\nmtls: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hami/refs/heads/main/authentication/hami-authentication.yml
summary_line: 0 schemes
tags:
- AI Computing
- CNCF
- GPU Virtualization
- Kubernetes
- GPU Sharing
- Scheduling
- Open Source
- Infrastructure
- Observability
- Heterogeneous Computing
---
