---
api_key_in: []
api_specs:
- filename: linode-account-api-openapi.yml
  format: yaml
  label: linode Account API
  slug: linode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-account-api-openapi.yml
- filename: linode-databases-api-openapi.yml
  format: yaml
  label: linode Databases API
  slug: linode-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-databases-api-openapi.yml
- filename: linode-domains-api-openapi.yml
  format: yaml
  label: linode Domains API
  slug: linode-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-domains-api-openapi.yml
- filename: linode-images-api-openapi.yml
  format: yaml
  label: linode Images API
  slug: linode-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-images-api-openapi.yml
- filename: linode-linode-instances-api-openapi.yml
  format: yaml
  label: linode Linode Instances API
  slug: linode-linode-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-linode-instances-api-openapi.yml
- filename: linode-linode-kubernetes-engine-lke-api-openapi.yml
  format: yaml
  label: linode Linode Kubernetes Engine (LKE) API
  slug: linode-linode-kubernetes-engine-lke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-linode-kubernetes-engine-lke-api-openapi.yml
- filename: linode-longview-api-openapi.yml
  format: yaml
  label: linode Longview API
  slug: linode-longview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-longview-api-openapi.yml
- filename: linode-managed-api-openapi.yml
  format: yaml
  label: linode Managed API
  slug: linode-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-managed-api-openapi.yml
- filename: linode-networking-api-openapi.yml
  format: yaml
  label: linode Networking API
  slug: linode-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-networking-api-openapi.yml
- filename: linode-nodebalancers-api-openapi.yml
  format: yaml
  label: linode NodeBalancers API
  slug: linode-nodebalancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-nodebalancers-api-openapi.yml
- filename: linode-object-storage-api-openapi.yml
  format: yaml
  label: linode Object Storage API
  slug: linode-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-object-storage-api-openapi.yml
- filename: linode-placement-groups-api-openapi.yml
  format: yaml
  label: linode Placement Groups API
  slug: linode-placement-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-placement-groups-api-openapi.yml
- filename: linode-profile-api-openapi.yml
  format: yaml
  label: linode Profile API
  slug: linode-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-profile-api-openapi.yml
- filename: linode-regions-api-openapi.yml
  format: yaml
  label: linode Regions API
  slug: linode-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-regions-api-openapi.yml
- filename: linode-stackscripts-api-openapi.yml
  format: yaml
  label: linode StackScripts API
  slug: linode-stackscripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-stackscripts-api-openapi.yml
- filename: linode-support-api-openapi.yml
  format: yaml
  label: linode Support API
  slug: linode-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-support-api-openapi.yml
- filename: linode-tags-api-openapi.yml
  format: yaml
  label: linode Tags API
  slug: linode-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-tags-api-openapi.yml
- filename: linode-volumes-api-openapi.yml
  format: yaml
  label: linode Volumes API
  slug: linode-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-volumes-api-openapi.yml
- filename: linode-vpcs-api-openapi.yml
  format: yaml
  label: linode VPCs API
  slug: linode-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/openapi/linode-vpcs-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Linode Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Linode secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Linode
provider_slug: linode
scheme_count: 2
schemes:
- description: A personal access token generated from the Linode Cloud Manager that grants access to the API based on the token's scopes.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/linode-api-v4-openapi.yml
  type: http
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://login.linode.com/oauth/authorize
    flow: authorizationCode
    scopes: 28
    tokenUrl: https://login.linode.com/oauth/token
  name: oauth
  sources:
  - openapi/linode-api-v4-openapi.yml
  type: oauth2
slug: linode-authentication
source_filename: linode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linode-api-v4-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: A personal access token generated from the Linode Cloud Manager that grants access\n    to the API based on the token's scopes.\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.linode.com/oauth/authorize\n    tokenUrl: https://login.linode.com/oauth/token\n    scopes: 28\n  description: OAuth 2.0 authentication for third-party applications.\n  sources:\n  - openapi/linode-api-v4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/authentication/linode-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags: []
---
