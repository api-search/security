---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loft-labs-platform-openapi-generated.yml
  format: yaml
  label: Loft Labs vCluster Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/_ae-authored/loft-labs-platform-openapi-generated.yml
- filename: loft-labs-vcluster-openapi-generated.yml
  format: yaml
  label: Loft Labs vCluster API
  slug: vcluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/_ae-authored/loft-labs-vcluster-openapi-generated.yml
auth_types: []
description: Authentication schemes published for Loft Labs vCluster
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Loft Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loft Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Loft Labs
provider_slug: loft-labs
scheme_count: 1
schemes:
- evidence: vCluster Platform can act as an OpenID Connect provider for other services, e.g. a self-hosted container registry using Harbor .
  how_to_obtain: Configure OIDC clients with clientId and clientSecret in the vCluster Platform configuration or via Kubernetes secrets.
  name: vCluster Platform OIDC
  type: oauth2
slug: loft-labs-authentication
source_filename: loft-labs-authentication.yml
source_heading: Authentication Profile
source_url: https://www.vcluster.com/docs/vcluster/configure/vcluster-yaml/control-plane/components/backing-store/database/external
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.vcluster.com/docs/vcluster/configure/vcluster-yaml/control-plane/components/backing-store/database/external\nsources:\n- https://www.vcluster.com/docs/vcluster/configure/vcluster-yaml/control-plane/components/backing-store/database/external\n- https://www.vcluster.com/docs/platform/administer/authentication/oidc-provider\n- https://www.vcluster.com/docs/vcluster\n- https://www.vcluster.com/docs/vcluster/quick-start/shared-nodes\ndescription: Authentication schemes published for Loft Labs vCluster\nschemes:\n- type: oauth2\n  name: vCluster Platform OIDC\n  evidence: vCluster Platform can act as an OpenID Connect provider for other services, e.g. a self-hosted container registry using Harbor .\n  how_to_obtain: Configure OIDC clients with clientId and clientSecret in the vCluster Platform configuration or via Kubernetes secrets.\ndocs: https://www.vcluster.com/docs/vcluster/configure/vcluster-yaml/control-plane/components/backing-store/database/external\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/authentication/loft-labs-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Cloud
- Kubernetes
- Multi-tenant
- Infrastructure
---
