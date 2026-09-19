---
anonymous_access: false
api_key_in:
- header
api_specs:
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
- filename: amazon-workspaces-web-browser-settings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Browser Settings API
  slug: amazon-workspaces-web-browser-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-browser-settings-api-openapi.yml
- filename: amazon-workspaces-web-identity-providers-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Identity Providers API
  slug: amazon-workspaces-web-identity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-identity-providers-api-openapi.yml
- filename: amazon-workspaces-web-ip-access-settings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Ip Access Settings API
  slug: amazon-workspaces-web-ip-access-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-ip-access-settings-api-openapi.yml
- filename: amazon-workspaces-web-network-settings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Network Settings API
  slug: amazon-workspaces-web-network-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-network-settings-api-openapi.yml
- filename: amazon-workspaces-web-portal-idp-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Portal Idp API
  slug: amazon-workspaces-web-portal-idp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-portal-idp-api-openapi.yml
- filename: amazon-workspaces-web-trust-stores-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web Trust Stores API
  slug: amazon-workspaces-web-trust-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-trust-stores-api-openapi.yml
- filename: amazon-workspaces-web-user-access-logging-settings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web User Access Logging Settings API
  slug: amazon-workspaces-web-user-access-logging-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-user-access-logging-settings-api-openapi.yml
- filename: amazon-workspaces-web-user-settings-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Web User Settings API
  slug: amazon-workspaces-web-user-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/openapi/amazon-workspaces-web-user-settings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
