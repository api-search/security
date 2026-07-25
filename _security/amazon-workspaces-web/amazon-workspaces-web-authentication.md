---
api_key_in:
- header
api_specs:
- filename: amazon-workspaces-web-browsersettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web BrowserSettings API
  slug: amazon-workspaces-web-browsersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-browsersettings-api-openapi.yml
- filename: amazon-workspaces-web-identityproviders-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web IdentityProviders API
  slug: amazon-workspaces-web-identityproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-identityproviders-api-openapi.yml
- filename: amazon-workspaces-web-ipaccesssettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web IpAccessSettings API
  slug: amazon-workspaces-web-ipaccesssettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-ipaccesssettings-api-openapi.yml
- filename: amazon-workspaces-web-networksettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web NetworkSettings API
  slug: amazon-workspaces-web-networksettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-networksettings-api-openapi.yml
- filename: amazon-workspaces-web-portalidp-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web PortalIdp API
  slug: amazon-workspaces-web-portalidp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-portalidp-api-openapi.yml
- filename: amazon-workspaces-web-portals-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Portals API
  slug: amazon-workspaces-web-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-portals-api-openapi.yml
- filename: amazon-workspaces-web-tags-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Tags API
  slug: amazon-workspaces-web-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-tags-api-openapi.yml
- filename: amazon-workspaces-web-truststores-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web TrustStores API
  slug: amazon-workspaces-web-truststores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-truststores-api-openapi.yml
- filename: amazon-workspaces-web-useraccessloggingsettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web UserAccessLoggingSettings API
  slug: amazon-workspaces-web-useraccessloggingsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-useraccessloggingsettings-api-openapi.yml
- filename: amazon-workspaces-web-usersettings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web UserSettings API
  slug: amazon-workspaces-web-usersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-usersettings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Workspaces Web Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon WorkSpaces Web secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-workspaces-web-openapi-original.yaml
  type: apiKey
slug: amazon-workspaces-web-authentication
source_filename: amazon-workspaces-web-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-workspaces-web-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-workspaces-web-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/authentication/amazon-workspaces-web-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
---
