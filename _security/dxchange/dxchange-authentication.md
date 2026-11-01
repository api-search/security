---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dxchange-openapi-generated.yml
  format: yaml
  label: DXchange.io API
  slug: dxchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dxchange/openapi/_ae-authored/dxchange-openapi-generated.yml
auth_types: []
description: Authentication methods described in the Transfer CFT documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dxchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: DXchange.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DXchange.io
provider_slug: dxchange
scheme_count: 2
schemes:
- evidence: 'Password authentication: synchronous communication'
  name: Password authentication
  type: http-basic
- evidence: SSO using SAML
  name: SSO using SAML
  type: other
slug: dxchange-authentication
source_filename: dxchange-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.axway.com/bundle/TransferCFT_36_UsersGuide_allOS_en_HTML5/page/Content/apis/api_authentication.htm
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.axway.com/bundle/TransferCFT_36_UsersGuide_allOS_en_HTML5/page/Content/apis/api_authentication.htm\nsources:\n- https://docs.axway.com/bundle/TransferCFT_36_UsersGuide_allOS_en_HTML5/page/Content/apis/api_authentication.htm\n- https://docs.axway.com/bundle/TransferCFT_310_allOS_en_HTML5/page/about_authentication_methods.html\n- https://docs.axway.com/bundle/TransferCFT_310_allOS_en_HTML5/page/client_authentication.html\n- https://docs.axway.com/bundle/TransferCFT_36_UsersGuide_allOS_en_HTML5/page/Content/Security/Tokens/use_saml.htm\ndescription: Authentication methods described in the Transfer CFT documentation.\nschemes:\n- type: http-basic\n  name: Password authentication\n  evidence: 'Password authentication: synchronous communication'\n- type: other\n  name: SSO using SAML\n  evidence: SSO using SAML\ndocs: https://docs.axway.com/bundle/TransferCFT_36_UsersGuide_allOS_en_HTML5/page/Content/apis/api_authentication.htm\n"
source_yaml_url: https://artifacts.apis.io/dxchange/authentication/dxchange-authentication.yml
summary_line: 2 schemes
tags:
- Integration
- API Management
- Managed File Transfer
- B2B Integration
- Enterprise Data
---
