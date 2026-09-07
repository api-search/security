---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloud-foundry-capi-v3-openapi.yaml
  format: yaml
  label: Cloud Foundry Cloud Controller API v3
  slug: capi-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-capi-v3-openapi.yaml
- filename: cloud-foundry-open-service-broker-api-openapi.yaml
  format: yaml
  label: Open Service Broker API
  slug: open-service-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-open-service-broker-api-openapi.yaml
- filename: cloud-foundry-apps-api-openapi.yml
  format: yaml
  label: Cloud Foundry Apps API
  slug: cloud-foundry-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-apps-api-openapi.yml
- filename: cloud-foundry-builds-api-openapi.yml
  format: yaml
  label: Cloud Foundry Builds API
  slug: cloud-foundry-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-builds-api-openapi.yml
- filename: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Foundry Cloud Controller API V3 API
  slug: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
- filename: cloud-foundry-deployments-api-openapi.yml
  format: yaml
  label: Cloud Foundry Deployments API
  slug: cloud-foundry-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-deployments-api-openapi.yml
- filename: cloud-foundry-jobs-api-openapi.yml
  format: yaml
  label: Cloud Foundry Jobs API
  slug: cloud-foundry-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-jobs-api-openapi.yml
- filename: cloud-foundry-organizations-api-openapi.yml
  format: yaml
  label: Cloud Foundry Organizations API
  slug: cloud-foundry-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-organizations-api-openapi.yml
- filename: cloud-foundry-service-instances-api-openapi.yml
  format: yaml
  label: Cloud Foundry Service Instances API
  slug: cloud-foundry-service-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-service-instances-api-openapi.yml
- filename: cloud-foundry-spaces-api-openapi.yml
  format: yaml
  label: Cloud Foundry Spaces API
  slug: cloud-foundry-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-spaces-api-openapi.yml
- filename: cloud-foundry-app-autoscaler-policy-api-openapi.yaml
  format: yaml
  label: Cloud Foundry App Autoscaler API
  slug: app-autoscaler
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-app-autoscaler-policy-api-openapi.yaml
auth_types:
- http
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cloud Foundry Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Cloud Foundry secures its APIs with http, mutualTLS, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Cloud Foundry
provider_slug: cloud-foundry
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-foundry-app-autoscaler-application-metric-api-openapi.yaml
  - openapi/cloud-foundry-app-autoscaler-policy-api-openapi.yaml
  - openapi/cloud-foundry-app-autoscaler-scaling-history-api-openapi.yaml
  - openapi/cloud-foundry-apps-api-openapi.yml
  - openapi/cloud-foundry-builds-api-openapi.yml
  - openapi/cloud-foundry-capi-v3-openapi.yaml
  - openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
  - openapi/cloud-foundry-deployments-api-openapi.yml
  - openapi/cloud-foundry-jobs-api-openapi.yml
  - openapi/cloud-foundry-organizations-api-openapi.yml
  - openapi/cloud-foundry-service-instances-api-openapi.yml
  - openapi/cloud-foundry-spaces-api-openapi.yml
  type: http
- description: Use the Instance Identity Credentials provided by the Cloud Foundry runtime
  name: mtls
  sources:
  - openapi/cloud-foundry-app-autoscaler-custom-metrics-api-openapi.yaml
  type: mutualTLS
- name: basicAuthentication
  scheme: basic
  sources:
  - openapi/cloud-foundry-app-autoscaler-custom-metrics-api-openapi.yaml
  - openapi/cloud-foundry-open-service-broker-api-openapi.yaml
  type: http
- flows:
  - authorizationUrl: https://uaa.cloudfoundry.local/api-oauth/dialog
    flow: implicit
    scopes: 7
  name: oauth
  sources:
  - openapi/cloud-foundry-capi-v3-openapi.yaml
  type: oauth2
slug: cloud-foundry-authentication
source_filename: cloud-foundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/cloud-foundry-app-autoscaler-application-metric-api-openapi.yaml, openapi/cloud-foundry-app-autoscaler-custom-metrics-api-openapi.yaml,\n  openapi/cloud-foundry-app-autoscaler-policy-api-openapi.yaml, openapi/cloud-foundry-app-autoscaler-scaling-history-api-openapi.yaml,\n  openapi/cloud-foundry-apps-api-openapi.yml, openapi/cloud-foundry-builds-api-openapi.yml, openapi/cloud-foundry-capi-v3-openapi.yaml,\n  openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml, openapi/cloud-foundry-deployments-api-openapi.yml,\n  openapi/cloud-foundry-jobs-api-openapi.yml, openapi/cloud-foundry-open-service-broker-api-openapi.yaml, openapi/cloud-foundry-organizations-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - mutualTLS\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cloud-foundry-app-autoscaler-application-metric-api-openapi.yaml\n\
  \  - openapi/cloud-foundry-app-autoscaler-policy-api-openapi.yaml\n  - openapi/cloud-foundry-app-autoscaler-scaling-history-api-openapi.yaml\n  - openapi/cloud-foundry-apps-api-openapi.yml\n  - openapi/cloud-foundry-builds-api-openapi.yml\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\n  - openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml\n  - openapi/cloud-foundry-deployments-api-openapi.yml\n  - openapi/cloud-foundry-jobs-api-openapi.yml\n  - openapi/cloud-foundry-organizations-api-openapi.yml\n  - openapi/cloud-foundry-service-instances-api-openapi.yml\n  - openapi/cloud-foundry-spaces-api-openapi.yml\n- name: mtls\n  type: mutualTLS\n  description: Use the Instance Identity Credentials provided by the Cloud Foundry runtime\n  sources:\n  - openapi/cloud-foundry-app-autoscaler-custom-metrics-api-openapi.yaml\n- name: basicAuthentication\n  type: http\n  scheme: basic\n  sources:\n  - openapi/cloud-foundry-app-autoscaler-custom-metrics-api-openapi.yaml\n  -\
  \ openapi/cloud-foundry-open-service-broker-api-openapi.yaml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://uaa.cloudfoundry.local/api-oauth/dialog\n    scopes: 7\n  sources:\n  - openapi/cloud-foundry-capi-v3-openapi.yaml\ndocs:\n- https://docs.cloudfoundry.org/uaa/\n- https://docs.cloudfoundry.org/api/uaa/\n- https://docs.cloudfoundry.org/concepts/architecture/uaa.html\n- https://github.com/cloudfoundry/uaa\nnote: 'Cloud Foundry does not run an identity service — it ships one. Every foundation deploys its own User Account\n  and Authentication (UAA) server at uaa.<system-domain>, an OAuth 2.0 / OpenID Connect authorization server with\n  SCIM 2.0 user and group management, and SAML/LDAP/OIDC federation. There is no central Cloud Foundry account,\n  no API key to obtain, and no signup: credentials belong to whoever runs the deployment you are calling. `cf oauth-token`\n  prints the current bearer JWT from an authenticated cf CLI session and\
  \ is the practical bridge from the CLI to\n  any HTTP client.\n\n  The four schemes below span the whole profile and are NOT interchangeable: the Cloud Controller takes UAA-issued\n  bearer JWTs; the App Autoscaler custom-metrics endpoint takes mutual TLS using the Instance Identity credentials\n  the runtime injects into the container (the only mTLS surface here, and a genuinely strong choice for an in-container\n  caller); the Open Service Broker contract takes HTTP Basic between platform and broker. Authorization then adds\n  a second axis — see scopes/cloud-foundry-scopes.yml.'\ndiscovery:\n  openid_configuration: https://uaa.<system-domain>/.well-known/openid-configuration\n  probed: false\n  note: 'Not probed: there is no public UAA instance. Every /.well-known/ path on every Foundation-controlled host\n    404s (well-known/cloud-foundry-well-known.yml).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/authentication/cloud-foundry-authentication.yml
summary_line: http/mutualTLS/oauth2 · 4 schemes
tags:
- Cloud Foundry Foundation
- Containers
- Multi-Cloud
- Open-Source
- Platform-as-a-Service
- Platform
---
