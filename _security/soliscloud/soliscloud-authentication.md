---
anonymous_access: false
api_key_in: []
api_specs:
- filename: soliscloud-openapi-generated.yml
  format: yaml
  label: Ginlong Technologies Co., Ltd. API
  slug: soliscloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soliscloud/openapi/_ae-authored/soliscloud-openapi-generated.yml
auth_types: []
description: Authentication methods for SolisCloud API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ginlong Technologies Co., Ltd. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ginlong Technologies Co., Ltd. declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ginlong Technologies Co., Ltd.
provider_slug: soliscloud
scheme_count: 2
schemes:
- evidence: Use your KeyID and KeySecret to generate a Custom HMAC-SHA1 signature, then call Data Access, Device Control, and other APIs accordingly.
  how_to_obtain: Retrieve your KeyID and KeySecret from the SolisCloud web portal after activation.
  name: HMAC Signature
  type: hmac
- evidence: Use your OAuth2.0 Access Token to call Data Access, Device Control, and other APIs.
  header: Authorization
  how_to_obtain: Obtain OAuth2.0 authorization from the plant owner and retrieve the Access Token.
  location: header
  name: OAuth2.0 Bearer Token
  type: http-bearer
slug: soliscloud-authentication
source_filename: soliscloud-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.soliscloud.com/guide/quick-start.html
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.soliscloud.com/guide/quick-start.html\nsources:\n- https://developer.soliscloud.com/guide/quick-start.html\n- https://developer.soliscloud.com/guide/quick-start\ndescription: Authentication methods for SolisCloud API\nschemes:\n- type: hmac\n  name: HMAC Signature\n  evidence: Use your KeyID and KeySecret to generate a Custom HMAC-SHA1 signature, then call Data Access, Device Control, and other APIs accordingly.\n  how_to_obtain: Retrieve your KeyID and KeySecret from the SolisCloud web portal after activation.\n- type: http-bearer\n  name: OAuth2.0 Bearer Token\n  evidence: Use your OAuth2.0 Access Token to call Data Access, Device Control, and other APIs.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain OAuth2.0 authorization from the plant owner and retrieve the Access Token.\ndocs: https://developer.soliscloud.com/guide/quick-start.html\n"
source_yaml_url: https://artifacts.apis.io/soliscloud/authentication/soliscloud-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Solar
- Monitoring
- Software-as-a-Service
- Renewable Energy
---
