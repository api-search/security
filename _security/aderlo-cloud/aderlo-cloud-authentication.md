---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aderlo-cloud-api-openapi.json
  format: json
  label: Aderlo Cloud public API API
  slug: aderlo-cloud-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aderlo-cloud/openapi/_original/aderlo-cloud-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Aderlo Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aderlo Cloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aderlo Cloud
provider_slug: aderlo-cloud
scheme_count: 1
schemes:
- flows:
    authorizationCode:
      authorizationUrl: https://aderlo.cloud/connect
      scopes:
        account: account tools
        agent: agent tools
        databases: databases tools
        dns: dns tools
        files: files tools
        mail: mail tools
      tokenUrl: https://aderlo.cloud/oauth/token
  type: oauth2
slug: aderlo-cloud-authentication
source_filename: aderlo-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://aderlo.cloud/openapi.json\nschemes:\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://aderlo.cloud/connect\n        tokenUrl: https://aderlo.cloud/oauth/token\n        scopes:\n          files: \"files tools\"\n          dns: \"dns tools\"\n          mail: \"mail tools\"\n          databases: \"databases tools\"\n          account: \"account tools\"\n          agent: \"agent tools\"\n"
source_yaml_url: https://artifacts.apis.io/aderlo-cloud/authentication/aderlo-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Hosting
- WooCommerce
- WordPress
- EU
- Managed
- Cloud
---
