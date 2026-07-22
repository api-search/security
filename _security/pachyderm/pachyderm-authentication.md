---
api_key_in: []
auth_types:
- oidc
- bearer-token
description: Pachyderm authenticates API/gRPC and pachctl clients with session tokens carried in gRPC metadata. Human users log in via OIDC (Pachyderm bundles a Dex identity provider); automation uses robot tokens. Authorization is RBAC — role bindings evaluated by the Auth service. Auth is activated per cluster (Enterprise feature) and rooted by a rotatable root token.
kind: authentication
layout: security
method: searched
name: Pachyderm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pachyderm secures its APIs with oidc and bearer-token across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pachyderm
provider_slug: pachyderm
scheme_count: 3
schemes:
- detail: GetOIDCLogin returns a browser login URL; pachctl auth login completes the OIDC flow and stores the resulting Pachyderm session token.
  flow: authorizationCode
  name: OIDC
  provider: Dex (embedded)
  source: https://github.com/pachyderm/dex
  type: openIdConnect
- detail: GetRobotToken mints a long-lived non-human token for CI/automation, scoped by the RBAC role bindings assigned to the robot principal.
  name: RobotToken
  scheme: bearer
  type: http
- detail: Cluster root credential established at auth Activate; rotatable via RotateRootToken.
  name: RootToken
  scheme: bearer
  type: http
slug: pachyderm-authentication
source_filename: pachyderm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/pachyderm/pachyderm/blob/master/src/auth/auth.proto\ndescription: >-\n  Pachyderm authenticates API/gRPC and pachctl clients with session tokens\n  carried in gRPC metadata. Human users log in via OIDC (Pachyderm bundles a\n  Dex identity provider); automation uses robot tokens. Authorization is\n  RBAC — role bindings evaluated by the Auth service. Auth is activated per\n  cluster (Enterprise feature) and rooted by a rotatable root token.\nsummary:\n  types: [oidc, bearer-token]\n  token_transport: grpc-metadata (authn-token)\n  authz: rbac\nschemes:\n  - name: OIDC\n    type: openIdConnect\n    provider: Dex (embedded)\n    flow: authorizationCode\n    detail: >-\n      GetOIDCLogin returns a browser login URL; pachctl auth login completes\n      the OIDC flow and stores the resulting Pachyderm session token.\n    source: https://github.com/pachyderm/dex\n  - name: RobotToken\n    type: http\n    scheme:\
  \ bearer\n    detail: >-\n      GetRobotToken mints a long-lived non-human token for CI/automation,\n      scoped by the RBAC role bindings assigned to the robot principal.\n  - name: RootToken\n    type: http\n    scheme: bearer\n    detail: >-\n      Cluster root credential established at auth Activate; rotatable via\n      RotateRootToken.\nrbac:\n  role_binding_rpcs: [ModifyRoleBinding, GetRoleBinding, GetRolesForPermission]\n  permission_rpcs: [Authorize, GetPermissions, GetPermissionsForPrincipal, WhoAmI]\n  resources: [cluster, project, repo, pipeline]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pachyderm/refs/heads/main/authentication/pachyderm-authentication.yml
summary_line: oidc/bearer-token · 3 schemes
tags:
- Company
- MLOps
- Data Versioning
- Data Pipelines
- Data Lineage
- Machine Learning
- Kubernetes
- gRPC
- Open Source
---
