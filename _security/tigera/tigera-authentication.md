---
api_key_in:
- header
api_specs:
- filename: tigera-apis-api-openapi.yml
  format: yaml
  label: Tigera APIS API
  slug: tigera-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-apis-api-openapi.yml
- filename: tigera-projectcalicoorg-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org API
  slug: tigera-projectcalicoorg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-api-openapi.yml
- filename: tigera-projectcalicoorg-v3-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org V3 API
  slug: tigera-projectcalicoorg-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-v3-api-openapi.yml
- filename: tigera-version-api-openapi.yml
  format: yaml
  label: Tigera Version API
  slug: tigera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-version-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
- openIdConnect
- mutualTLS
description: Tigera has four distinct authentication surfaces and none of them are declared in an OpenAPI securityScheme — the published Swagger 2.0 definition for the Calico API carries no securityDefinitions block at all, because the API is a Kubernetes aggregated API server that inherits the host cluster's authenticators. This profile was written from the documentation and from probed OAuth metadata, not derived from the spec.
kind: authentication
layout: security
method: searched
name: Tigera Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Tigera secures its APIs with http, apiKey, oauth2, openIdConnect, and mutualTLS across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Tigera
provider_slug: tigera
scheme_count: 6
schemes:
- description: 'The Calico aggregated API server sits behind the cluster''s kube-apiserver, which performs authentication. Callers present a Kubernetes ServiceAccount token or an OIDC ID token as `Authorization: Bearer <token>`. Authorization is Kubernetes RBAC over projectcalico.org/v3 resources, extended by Calico''s tier-scoped policy RBAC (a subject needs get on the tier plus the verb on the policy resource within that tier).'
  docs: https://docs.tigera.io/calico/latest/operations/install-apiserver
  name: KubernetesBearerToken
  scheme: bearer
  sources:
  - documentation
  surface: Calico API (projectcalico.org/v3)
  type: http
- description: Client-certificate authentication to the kube-apiserver, the default for kubeconfig credentials created by kubeadm and most managed Kubernetes distributions. calicoctl and kubectl both read these from kubeconfig.
  docs: https://docs.tigera.io/calico/latest/operations/calicoctl/configure/kdd
  name: KubernetesClientCertificate
  sources:
  - documentation
  surface: Calico API (projectcalico.org/v3)
  type: mutualTLS
- description: In etcdv3 datastore deployments calicoctl authenticates directly to etcd with ETCD_CERT_FILE / ETCD_KEY_FILE / ETCD_CA_CERT_FILE, or with ETCD_USERNAME / ETCD_PASSWORD.
  docs: https://docs.tigera.io/calico/latest/operations/calicoctl/configure/etcd
  name: EtcdDatastoreCredentials
  sources:
  - documentation
  surface: Calico API — etcdv3 datastore mode
  type: mutualTLS
- description: Read-only, organization-scoped API keys generated in the Calico Cloud web console under Settings > API Keys, with a chosen validity period. The key value is shown exactly once at creation and cannot be retrieved afterwards. Creating one requires the Admin + Usage Metrics roles or the Owner role. The console emits a ready-made command per key. Tigera does not publish the header name in public documentation, so it is recorded as unknown rather than guessed.
  docs: https://docs.tigera.io/calico-cloud/operations/usage-api
  in: header
  name: CalicoCloudUsageApiKey
  parameter_name: null
  sources:
  - documentation
  surface: Calico Cloud Usage API
  type: apiKey
- description: The Calico Cloud console authenticates users over OIDC (Auth0), with Google social login among the supported options, mapped onto the predefined roles Owner, Admin, Security and Viewer.
  docs: https://docs.tigera.io/calico-cloud/users/user-management
  name: CalicoCloudConsoleSSO
  sources:
  - documentation
  surface: Calico Cloud web console
  type: openIdConnect
- description: OAuth 2.1 authorization-code with PKCE (S256) for the remote MCP server on www.tigera.io. Public clients (token_endpoint_auth_method none) identified by client-ID metadata document; bearer token presented in the Authorization header; single scope `mcp`.
  detail: scopes/tigera-scopes.yml
  flows:
  - authorizationUrl: https://www.tigera.io/oauth/authorize
    flow: authorizationCode
    scopes:
    - mcp
    tokenUrl: https://www.tigera.io/oauth/token
  name: TigeraMCPOAuth
  sources:
  - https://www.tigera.io/.well-known/oauth-authorization-server
  surface: Tigera MCP server
  type: oauth2
slug: tigera-authentication
source_filename: tigera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: >-\n  https://docs.tigera.io/calico/latest/operations/install-apiserver,\n  https://docs.tigera.io/calico-cloud/operations/usage-api,\n  https://docs.tigera.io/calico-cloud/users/user-management,\n  https://www.tigera.io/.well-known/oauth-authorization-server\ndocs: https://docs.tigera.io/calico-cloud/users/user-management\ndescription: >-\n  Tigera has four distinct authentication surfaces and none of them are declared in an OpenAPI\n  securityScheme — the published Swagger 2.0 definition for the Calico API carries no\n  securityDefinitions block at all, because the API is a Kubernetes aggregated API server that\n  inherits the host cluster's authenticators. This profile was written from the documentation\n  and from probed OAuth metadata, not derived from the spec.\nsummary:\n  types: [http, apiKey, oauth2, openIdConnect, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  derived_from_openapi: false\n\
  \  openapi_security_definitions: 0\nschemes:\n- name: KubernetesBearerToken\n  surface: Calico API (projectcalico.org/v3)\n  type: http\n  scheme: bearer\n  description: >-\n    The Calico aggregated API server sits behind the cluster's kube-apiserver, which performs\n    authentication. Callers present a Kubernetes ServiceAccount token or an OIDC ID token as\n    `Authorization: Bearer <token>`. Authorization is Kubernetes RBAC over\n    projectcalico.org/v3 resources, extended by Calico's tier-scoped policy RBAC (a\n    subject needs get on the tier plus the verb on the policy resource within that tier).\n  docs: https://docs.tigera.io/calico/latest/operations/install-apiserver\n  sources: [documentation]\n- name: KubernetesClientCertificate\n  surface: Calico API (projectcalico.org/v3)\n  type: mutualTLS\n  description: >-\n    Client-certificate authentication to the kube-apiserver, the default for kubeconfig\n    credentials created by kubeadm and most managed Kubernetes distributions.\
  \ calicoctl and\n    kubectl both read these from kubeconfig.\n  docs: https://docs.tigera.io/calico/latest/operations/calicoctl/configure/kdd\n  sources: [documentation]\n- name: EtcdDatastoreCredentials\n  surface: Calico API — etcdv3 datastore mode\n  type: mutualTLS\n  description: >-\n    In etcdv3 datastore deployments calicoctl authenticates directly to etcd with\n    ETCD_CERT_FILE / ETCD_KEY_FILE / ETCD_CA_CERT_FILE, or with ETCD_USERNAME / ETCD_PASSWORD.\n  docs: https://docs.tigera.io/calico/latest/operations/calicoctl/configure/etcd\n  sources: [documentation]\n- name: CalicoCloudUsageApiKey\n  surface: Calico Cloud Usage API\n  type: apiKey\n  in: header\n  description: >-\n    Read-only, organization-scoped API keys generated in the Calico Cloud web console under\n    Settings > API Keys, with a chosen validity period. The key value is shown exactly once at\n    creation and cannot be retrieved afterwards. Creating one requires the Admin + Usage Metrics\n    roles or the\
  \ Owner role. The console emits a ready-made command per key. Tigera does not\n    publish the header name in public documentation, so it is recorded as unknown rather than\n    guessed.\n  parameter_name: null\n  docs: https://docs.tigera.io/calico-cloud/operations/usage-api\n  sources: [documentation]\n- name: CalicoCloudConsoleSSO\n  surface: Calico Cloud web console\n  type: openIdConnect\n  description: >-\n    The Calico Cloud console authenticates users over OIDC (Auth0), with Google social login\n    among the supported options, mapped onto the predefined roles Owner, Admin, Security and\n    Viewer.\n  docs: https://docs.tigera.io/calico-cloud/users/user-management\n  sources: [documentation]\n- name: TigeraMCPOAuth\n  surface: Tigera MCP server\n  type: oauth2\n  description: >-\n    OAuth 2.1 authorization-code with PKCE (S256) for the remote MCP server on www.tigera.io.\n    Public clients (token_endpoint_auth_method none) identified by client-ID metadata document;\n    bearer\
  \ token presented in the Authorization header; single scope `mcp`.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.tigera.io/oauth/authorize\n    tokenUrl: https://www.tigera.io/oauth/token\n    scopes: [mcp]\n  detail: scopes/tigera-scopes.yml\n  sources: [https://www.tigera.io/.well-known/oauth-authorization-server]\ngaps:\n- >-\n  The published Calico Swagger 2.0 document declares no securityDefinitions and applies no\n  security to any of its 261 operations. A generated client or an agent reading only the spec\n  has no machine-readable signal about how to authenticate.\n- >-\n  The Calico Cloud Usage API's authentication header name and base URL are not published; both\n  are only visible inside the authenticated console.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://docs.tigera.io/calico-cloud/operations/usage-api\n    status: 200\n  - url: https://www.tigera.io/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://docs.tigera.io/json/calico-api-swagger.json\n\
  \    status: 200\n    finding: securityDefinitions absent\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/authentication/tigera-authentication.yml
summary_line: http/apiKey/oauth2/openIdConnect/mutualTLS · 6 schemes
tags:
- Company
- Kubernetes
- Networking
- Network Security
- Container Security
- Cloud Native
- Observability
- Microsegmentation
- Zero Trust
- eBPF
- Open Source
---
