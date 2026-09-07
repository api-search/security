---
anonymous_access: false
api_key_in: []
api_specs:
- filename: calico-bgpconfiguration-api-openapi.yml
  format: yaml
  label: Calico BGPConfiguration API
  slug: calico-bgpconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgpconfiguration-api-openapi.yml
- filename: calico-bgppeer-api-openapi.yml
  format: yaml
  label: Calico BGPPeer API
  slug: calico-bgppeer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgppeer-api-openapi.yml
- filename: calico-globalnetworkpolicy-api-openapi.yml
  format: yaml
  label: Calico GlobalNetworkPolicy API
  slug: calico-globalnetworkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-globalnetworkpolicy-api-openapi.yml
- filename: calico-hostendpoint-api-openapi.yml
  format: yaml
  label: Calico HostEndpoint API
  slug: calico-hostendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-hostendpoint-api-openapi.yml
- filename: calico-ippool-api-openapi.yml
  format: yaml
  label: Calico IPPool API
  slug: calico-ippool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-ippool-api-openapi.yml
- filename: calico-networkpolicy-api-openapi.yml
  format: yaml
  label: Calico NetworkPolicy API
  slug: calico-networkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-networkpolicy-api-openapi.yml
- filename: calico-profile-api-openapi.yml
  format: yaml
  label: Calico Profile API
  slug: calico-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-profile-api-openapi.yml
auth_types:
- http
- mutualTLS
description: Calico's API has no credential of its own. It is served by the operator's Kubernetes API server, so authentication is whatever that cluster does — bearer token or client certificate — and authorization is Kubernetes RBAC over the projectcalico.org API group. There is no API key to provision, no OAuth flow on the API, no signup and no account. That is the single most useful fact about auth here, and the OpenAPI's lone BearerAuth scheme understates it.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Calico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calico secures its APIs with http and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Calico
provider_slug: calico
scheme_count: 2
schemes:
- bearerFormat: JWT
  declared_in_spec: true
  description: 'Kubernetes service account bearer token, or any token the cluster''s configured authenticator accepts (OIDC, webhook, static). Sent as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/calico-bgpconfiguration-api-openapi.yml
  - openapi/calico-bgppeer-api-openapi.yml
  - openapi/calico-globalnetworkpolicy-api-openapi.yml
  - openapi/calico-hostendpoint-api-openapi.yml
  - openapi/calico-ippool-api-openapi.yml
  - openapi/calico-networkpolicy-api-openapi.yml
  - openapi/calico-profile-api-openapi.yml
  type: http
- declared_in_spec: false
  description: Kubernetes client-certificate authentication (the kubeconfig client-certificate-data / client-key-data pair). Equally valid against this API and used by most operator tooling, including calicoctl through the standard kubeconfig.
  name: ClientCertificate
  source: Kubernetes API server contract, inherited. Not declared in openapi/.
  spec_gap: true
  type: mutualTLS
slug: calico-authentication
source_filename: calico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  openapi/*.yml (securitySchemes) enriched from\n  https://docs.tigera.io/calico/latest/getting-started/kubernetes/hardway/end-user-rbac ,\n  https://docs.tigera.io/calico/latest/network-policy/policy-tiers/rbac-tiered-policies ,\n  https://docs.tigera.io/calico/latest/reference/etcd-rbac/ ,\n  https://www.tigera.io/.well-known/oauth-authorization-server/\ndocs: https://docs.tigera.io/calico/latest/getting-started/kubernetes/hardway/end-user-rbac\ndescription: >-\n  Calico's API has no credential of its own. It is served by the operator's Kubernetes API server,\n  so authentication is whatever that cluster does — bearer token or client certificate — and\n  authorization is Kubernetes RBAC over the projectcalico.org API group. There is no API key to\n  provision, no OAuth flow on the API, no signup and no account. That is the single most useful fact\n  about auth here, and the OpenAPI's lone BearerAuth scheme understates\
  \ it.\nsummary:\n  types:\n  - http\n  - mutualTLS\n  authorization_model: kubernetes-rbac\n  api_keys: false\n  oauth_on_api: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Kubernetes service account bearer token, or any token the cluster's configured authenticator\n    accepts (OIDC, webhook, static). Sent as `Authorization: Bearer <token>`.\n  declared_in_spec: true\n  sources:\n  - openapi/calico-bgpconfiguration-api-openapi.yml\n  - openapi/calico-bgppeer-api-openapi.yml\n  - openapi/calico-globalnetworkpolicy-api-openapi.yml\n  - openapi/calico-hostendpoint-api-openapi.yml\n  - openapi/calico-ippool-api-openapi.yml\n  - openapi/calico-networkpolicy-api-openapi.yml\n  - openapi/calico-profile-api-openapi.yml\n- name: ClientCertificate\n  type: mutualTLS\n  description: >-\n    Kubernetes client-certificate authentication (the kubeconfig client-certificate-data /\n    client-key-data pair). Equally valid against this\
  \ API and used by most operator tooling,\n    including calicoctl through the standard kubeconfig.\n  declared_in_spec: false\n  spec_gap: true\n  source: Kubernetes API server contract, inherited. Not declared in openapi/.\nauthorization:\n  model: Kubernetes RBAC\n  api_group: projectcalico.org\n  docs: https://docs.tigera.io/calico/latest/getting-started/kubernetes/hardway/end-user-rbac\n  resources:\n  - networkpolicies\n  - globalnetworkpolicies\n  - stagednetworkpolicies\n  - stagedglobalnetworkpolicies\n  - stagedkubernetesnetworkpolicies\n  - networksets\n  - globalnetworksets\n  - ippools\n  - ipreservations\n  - bgppeers\n  - bgpconfigurations\n  - bgpfilters\n  - hostendpoints\n  - profiles\n  - tiers\n  - felixconfigurations\n  - clusterinformations\n  - caliconodestatuses\n  - kubecontrollersconfigurations\n  verbs: [get, list, watch, create, update, patch, delete]\n  tiered_policy_note: >-\n    Policy tiers add a second RBAC dimension: access to a policy is granted through\
  \ the `tiers`\n    resource as well as the policy resource itself, so a caller can hold full rights on\n    networkpolicies and still be refused inside a tier. See\n    https://docs.tigera.io/calico/latest/network-policy/policy-tiers/rbac-tiered-policies\n  cross_group_note: >-\n    Configuring an authenticated BGP peer requires RBAC on core/v1 Secrets as well, because\n    BGPPeer.spec.password.secretKeyRef points out of the projectcalico.org group. See\n    data-model/calico-data-model.yml.\n  failure_mode: >-\n    403 Forbidden with a Kubernetes metav1.Status body. NOT declared in openapi/ — see\n    errors/calico-problem-types.yml.\ndatastore_auth:\n  note: >-\n    On the legacy etcdv3 datastore (rather than the Kubernetes API datastore), Calico components\n    authenticate to etcd with their own TLS client certificates and etcd RBAC users/roles. That is a\n    component-to-datastore credential, not a client-facing one.\n  docs: https://docs.tigera.io/calico/latest/reference/etcd-rbac/\n\
  unrelated_oauth_surface:\n  note: >-\n    www.tigera.io publishes an RFC 8414 OAuth authorization server (scope `mcp`) fronting Tigera's\n    MCP server. It has nothing to do with authenticating to the Calico API. Recorded here only so it\n    is not mistaken for one. See scopes/calico-scopes.yml and mcp/calico-mcp.yml.\nagent_guidance: >-\n  Use the ambient cluster credential — an in-cluster service account token at\n  /var/run/secrets/kubernetes.io/serviceaccount/token, or the caller's kubeconfig. Do not look for a\n  Calico API key; none exists. Ensure the service account's Role/ClusterRole grants the verbs you\n  intend on the projectcalico.org resources above, plus the tier if tiered policy is in use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/authentication/calico-authentication.yml
summary_line: http/mutualTLS · 2 schemes
tags:
- CNI
- Containers
- eBPF
- Kubernetes
- Network Policy
- Network Security
- Networking
- Open-Source
- Service Mesh
---
