---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-arc-machines-api-openapi.yml
  format: yaml
  label: Azure Arc Machines API
  slug: microsoft-azure-arc-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machines-api-openapi.yml
- filename: microsoft-azure-arc-connectedclusters-api-openapi.yml
  format: yaml
  label: Azure Arc Connected Clusters API
  slug: microsoft-azure-arc-connectedclusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-connectedclusters-api-openapi.yml
- filename: microsoft-azure-arc-extensions-api-openapi.yml
  format: yaml
  label: Azure Arc Extensions API
  slug: microsoft-azure-arc-extensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-extensions-api-openapi.yml
- filename: microsoft-azure-arc-gateways-api-openapi.yml
  format: yaml
  label: Azure Arc Gateways API
  slug: microsoft-azure-arc-gateways-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-gateways-api-openapi.yml
- filename: microsoft-azure-arc-licenseprofiles-api-openapi.yml
  format: yaml
  label: Azure Arc License Profiles API
  slug: microsoft-azure-arc-licenseprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-licenseprofiles-api-openapi.yml
- filename: microsoft-azure-arc-licenses-api-openapi.yml
  format: yaml
  label: Azure Arc Licenses API
  slug: microsoft-azure-arc-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-licenses-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Extensions API
  slug: microsoft-azure-arc-machineextensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-setup-api-openapi.yml
  format: yaml
  label: Azure Arc MachineExtensions Setup API
  slug: microsoft-azure-arc-machineextensions-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-setup-api-openapi.yml
- filename: microsoft-azure-arc-machineextensions-upgrade-api-openapi.yml
  format: yaml
  label: Azure Arc MachineExtensions Upgrade API
  slug: microsoft-azure-arc-machineextensions-upgrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineextensions-upgrade-api-openapi.yml
- filename: microsoft-azure-arc-machinenetworkprofile-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Network Profile API
  slug: microsoft-azure-arc-machinenetworkprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machinenetworkprofile-api-openapi.yml
- filename: microsoft-azure-arc-machineruncommands-api-openapi.yml
  format: yaml
  label: Azure Arc Machine Run Commands API
  slug: microsoft-azure-arc-machineruncommands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-machineruncommands-api-openapi.yml
- filename: microsoft-azure-arc-networksecurityperimeterconfiguration-api-openapi.yml
  format: yaml
  label: Azure Arc Network Security Perimeter Configuration API
  slug: microsoft-azure-arc-networksecurityperimeterconfiguration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-networksecurityperimeterconfiguration-api-openapi.yml
- filename: microsoft-azure-arc-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Arc Private Link Resources API
  slug: microsoft-azure-arc-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-privatelinkresources-api-openapi.yml
- filename: microsoft-azure-arc-settings-api-openapi.yml
  format: yaml
  label: Azure Arc Settings API
  slug: microsoft-azure-arc-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-settings-api-openapi.yml
- filename: microsoft-azure-arc-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Arc Subscriptions API
  slug: microsoft-azure-arc-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-subscriptions-api-openapi.yml
- filename: microsoft-azure-arc-vmapplications-api-openapi.yml
  format: yaml
  label: Azure Arc Vm Applications API
  slug: microsoft-azure-arc-vmapplications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-vmapplications-api-openapi.yml
- filename: microsoft-azure-arc-operations-api-openapi.yml
  format: yaml
  label: Azure Arc Operations API
  slug: microsoft-azure-arc-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-operations-api-openapi.yml
- filename: microsoft-azure-arc-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Arc Private Endpoint Connections API
  slug: microsoft-azure-arc-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-arc/openapi/microsoft-azure-arc-private-endpoint-connections-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Azure Arc Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Arc secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Arc
provider_slug: microsoft-azure-arc
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-arc-hybridcompute-openapi.yml
  type: oauth2
slug: microsoft-azure-arc-authentication
source_filename: microsoft-azure-arc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-azure-arc-hybridcompute-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-arc-hybridcompute-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-arc/authentication/microsoft-azure-arc-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Arc
- Hybrid Cloud
- Kubernetes
- Multi-Cloud
- Server Management
---
