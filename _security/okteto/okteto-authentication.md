---
anonymous_access: false
api_key_in: []
api_specs:
- filename: okteto-applications-api-openapi.yml
  format: yaml
  label: Okteto Applications API
  slug: okteto-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/okteto/openapi/okteto-applications-api-openapi.yml
- filename: okteto-namespaces-api-openapi.yml
  format: yaml
  label: Okteto Namespaces API
  slug: okteto-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/okteto/openapi/okteto-namespaces-api-openapi.yml
auth_types: []
description: Authentication schemes for Okteto as documented in the provided pages
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Okteto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okteto declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Okteto
provider_slug: okteto
scheme_count: 3
schemes:
- evidence: Okteto supports any identity provider that implements the OpenID Connect standard.
  flows:
  - authorization_code
  how_to_obtain: Create an OpenID Connect application with your identity provider and configure clientId and clientSecret in Okteto's Helm configuration.
  name: OpenID Connect
  scopes:
  - openid
  - email
  - profile
  type: oauth2
- evidence: Azure Cloud Credentials let the commands in your Okteto Manifests authenticate to Microsoft Azure with the identity of your Okteto cluster, without client secrets.
  how_to_obtain: Configure Azure Cloud Credentials in Okteto Admin Dashboard with Tenant ID, Client ID, Audience JWT Claim (api://AzureADTokenExchange), and Authority Host.
  name: Azure Workload ID
  type: jwt
- evidence: The kubeconfig provided by Okteto uses a credential plugin to authenticate access your Kubernetes cluster.
  how_to_obtain: Use 'okteto kubeconfig' command or download credentials from Okteto dashboard Settings > Setup section.
  name: Kubernetes Credential Plugin
  type: other
slug: okteto-authentication
source_filename: okteto-authentication.yml
source_heading: Authentication Profile
source_url: https://www.okteto.com/docs/self-hosted/install/auth/openid-connect
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://www.okteto.com/docs/self-hosted/install/auth/openid-connect\nsources:\n- https://www.okteto.com/docs/self-hosted/install/auth/openid-connect\n- https://www.okteto.com/docs/1.50/self-hosted/install/auth/openid-connect\n- https://www.okteto.com/docs/1.50/admin/cloud-credentials/azure-cloud-credentials\n- https://www.okteto.com/docs/1.43/core/credentials/kubernetes-credentials\ndescription: Authentication schemes for Okteto as documented in the provided pages\nschemes:\n- type: oauth2\n  name: OpenID Connect\n  evidence: Okteto supports any identity provider that implements the OpenID Connect standard.\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create an OpenID Connect application with your identity provider and configure clientId and clientSecret in Okteto's Helm configuration.\n- type: jwt\n  name: Azure Workload\
  \ ID\n  evidence: Azure Cloud Credentials let the commands in your Okteto Manifests authenticate to Microsoft Azure with the identity of your Okteto\n    cluster, without client secrets.\n  how_to_obtain: Configure Azure Cloud Credentials in Okteto Admin Dashboard with Tenant ID, Client ID, Audience JWT Claim (api://AzureADTokenExchange),\n    and Authority Host.\n- type: other\n  name: Kubernetes Credential Plugin\n  evidence: The kubeconfig provided by Okteto uses a credential plugin to authenticate access your Kubernetes cluster.\n  how_to_obtain: Use 'okteto kubeconfig' command or download credentials from Okteto dashboard Settings > Setup section.\ndocs: https://www.okteto.com/docs/self-hosted/install/auth/openid-connect, https://www.okteto.com/docs/1.50/self-hosted/install/auth/openid-connect,\n  https://www.okteto.com/docs/1.50/admin/cloud-credentials/azure-cloud-credentials, https://www.okteto.com/docs/1.43/core/credentials/kubernetes-credentials\nnote: 'The pages describe authentication\
  \ for different contexts: OpenID Connect for user authentication to Okteto, Azure Workload ID for cloud\n  credentials, and Kubernetes credential plugin for cluster access.'\n"
source_yaml_url: https://artifacts.apis.io/okteto/authentication/okteto-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Kubernetes
- Development Environments
- Cloud Native
- Developer Tools
- Preview Environments
- AI Agents
- CLI
---
