---
api_key_in:
- header
api_specs:
- filename: mithril-api-keys-api-openapi.yml
  format: yaml
  label: Mithril API Keys API
  slug: mithril-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-api-keys-api-openapi.yml
- filename: mithril-image-versions-api-openapi.yml
  format: yaml
  label: Mithril image versions API
  slug: mithril-image-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-image-versions-api-openapi.yml
- filename: mithril-instance-types-api-openapi.yml
  format: yaml
  label: Mithril instance types API
  slug: mithril-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-instance-types-api-openapi.yml
- filename: mithril-instances-api-openapi.yml
  format: yaml
  label: Mithril instances API
  slug: mithril-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-instances-api-openapi.yml
- filename: mithril-kubernetes-clusters-api-openapi.yml
  format: yaml
  label: Mithril kubernetes clusters API
  slug: mithril-kubernetes-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-kubernetes-clusters-api-openapi.yml
- filename: mithril-lifecycle-scripts-api-openapi.yml
  format: yaml
  label: Mithril lifecycle scripts API
  slug: mithril-lifecycle-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-lifecycle-scripts-api-openapi.yml
- filename: mithril-pricing-api-openapi.yml
  format: yaml
  label: Mithril pricing API
  slug: mithril-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-pricing-api-openapi.yml
- filename: mithril-profile-api-openapi.yml
  format: yaml
  label: Mithril profile API
  slug: mithril-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-profile-api-openapi.yml
- filename: mithril-projects-api-openapi.yml
  format: yaml
  label: Mithril projects API
  slug: mithril-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-projects-api-openapi.yml
- filename: mithril-quotas-api-openapi.yml
  format: yaml
  label: Mithril quotas API
  slug: mithril-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-quotas-api-openapi.yml
- filename: mithril-reservations-api-openapi.yml
  format: yaml
  label: Mithril reservations API
  slug: mithril-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-reservations-api-openapi.yml
- filename: mithril-spot-api-openapi.yml
  format: yaml
  label: Mithril spot API
  slug: mithril-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-spot-api-openapi.yml
- filename: mithril-ssh-keys-api-openapi.yml
  format: yaml
  label: Mithril SSH Keys API
  slug: mithril-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-ssh-keys-api-openapi.yml
- filename: mithril-volumes-api-openapi.yml
  format: yaml
  label: Mithril volumes API
  slug: mithril-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-volumes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mithril Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mithril secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mithril
provider_slug: mithril
scheme_count: 1
schemes:
- bearerFormat: fkey_<key>
  docs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys
  header: 'Authorization: Bearer fkey_<key>'
  name: MithrilAPIKey
  scheme: bearer
  sources:
  - openapi/mithril-compute-openapi-original.json
  type: http
slug: mithril-authentication
source_filename: mithril-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/mithril-compute-openapi-original.json\ndocs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: MithrilAPIKey\n  type: http\n  scheme: bearer\n  bearerFormat: fkey_<key>\n  header: 'Authorization: Bearer fkey_<key>'\n  docs: https://docs.mithril.ai/compute-api/compute-api-reference/api-keys\n  sources:\n  - openapi/mithril-compute-openapi-original.json\noauth_identity:\n  note: >-\n    Separately, the Mithril console/CLI sign-in uses OAuth 2.0 / OIDC at\n    login.mithril.ai (authorization_code, client_credentials, refresh_token,\n    device_code grants; scopes openid, profile, email, offline_access). This is\n    account identity, not the API's request auth (which is the fkey_ bearer key).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/authentication/mithril-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- GPU Cloud
- AI Infrastructure
- Machine-Learning
- Cloud Computing
- Compute
- Spot Instances
- Kubernetes
- GPU
---
