---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildpacks-kpack-swagger.json
  format: json
  label: kpack
  slug: kpack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks/refs/heads/main/openapi/buildpacks-kpack-swagger.json
auth_types: []
description: Cloud Native Buildpacks exposes three distinct authentication postures, none of them an API-key or OAuth program run by the project itself. Read access to the Buildpack Registry is fully anonymous; write access to the registry is delegated to GitHub identity; and the kpack CRD API inherits whatever the Kubernetes API server enforces. The kpack Swagger document declares no `securityDefinitions`, which is normal for a Kubernetes aggregated/CRD spec and is NOT an absence of auth — the cluster enforces it.
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Buildpacks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Native Buildpacks declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud Native Buildpacks
provider_slug: buildpacks
scheme_count: 0
schemes: []
slug: buildpacks-authentication
source_filename: buildpacks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://github.com/buildpacks/registry-api (README + config/routes.rb), anonymous probes of\n  https://registry.buildpacks.io/api/v1/*, openapi/buildpacks-kpack-swagger.json, and\n  https://buildpacks.io/docs/for-buildpack-authors/how-to/distribute-buildpacks/publish-buildpack/\nprovider: Cloud Native Buildpacks\nproviderId: buildpacks\ndescription: >-\n  Cloud Native Buildpacks exposes three distinct authentication postures, none of them an\n  API-key or OAuth program run by the project itself. Read access to the Buildpack Registry is fully\n  anonymous; write access to the registry is delegated to GitHub identity; and the kpack CRD API\n  inherits whatever the Kubernetes API server enforces. The kpack Swagger document declares no\n  `securityDefinitions`, which is normal for a Kubernetes aggregated/CRD spec and is NOT an absence\n  of auth — the cluster enforces it.\ndocs: https://buildpacks.io/docs/for-buildpack-authors/how-to/distribute-buildpacks/publish-buildpack/\n\
  surfaces:\n- api: Buildpack Registry API (read)\n  base_url: https://registry.buildpacks.io/api/v1\n  scheme: none\n  required: false\n  verified: probed\n  evidence: >-\n    GET https://registry.buildpacks.io/api/v1/search?matches=java returned HTTP 200 with a JSON body\n    with no credential of any kind on 2026-09-05. GET .../buildpacks/heroku/nodejs likewise 200.\n  note: >-\n    All three documented read operations (search, version list, version info) are public and\n    unauthenticated. No API key, token, or account is issued by the project.\n- api: Buildpack Registry (write / publish)\n  scheme: delegated-oauth\n  provider: GitHub\n  required: true\n  verified: searched\n  evidence: >-\n    https://buildpacks.io/docs/for-buildpack-authors/how-to/distribute-buildpacks/publish-buildpack/\n    — \"pack buildpack register example/my-cnb ... This will open GitHub in a browser and may ask you\n    to authenticate with GitHub.\"\n  note: >-\n    Publication is not an HTTP write against\
  \ registry.buildpacks.io. It is a structured GitHub Issue\n    opened against the registry index; the authenticated GitHub user becomes the owner of the\n    buildpack namespace on first publish. Namespace ownership changes are made by pull request to\n    https://github.com/buildpacks/registry-namespaces.\n- api: kpack (kpack.io/v1alpha1 CRD API)\n  scheme: kubernetes\n  mechanisms:\n  - bearer token (ServiceAccount / OIDC)\n  - client certificate\n  - whatever authenticators the cluster's API server is configured with\n  authorization: Kubernetes RBAC on the kpack.io API group\n  required: true\n  verified: derived\n  evidence: >-\n    openapi/buildpacks-kpack-swagger.json declares no `securityDefinitions`; every path is rooted at\n    /apis/kpack.io/v1alpha1/ and is therefore served by the Kubernetes API server, which\n    authenticates and authorizes the request before the kpack controller sees it.\n  note: >-\n    There is no CNB-issued credential here. An agent calling kpack authenticates\
  \ to the customer's\n    own cluster, not to buildpacks.io.\noauth2: false\napi_keys: false\nscopes_artifact: null\nscopes_note: >-\n  No OAuth 2.0 scope surface exists to derive. derive-oauth-scopes.py reported 0 oauth2\n  securitySchemes on 2026-09-05; scopes/ is deliberately absent rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildpacks/refs/heads/main/authentication/buildpacks-authentication.yml
summary_line: 0 schemes
tags:
- Build Tools
- CI/CD
- Cloud-Native
- CNCF
- Container Images
- Containers
- OCI
- Open-Source
---
