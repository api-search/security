---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paysimple-openapi-generated.yml
  format: yaml
  label: PaySimple API
  slug: paysimple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paysimple/openapi/_ae-authored/paysimple-openapi-generated.yml
auth_types: []
description: PaySimple requires an Authorization Header for each request. Merchant credentials use a custom "basic" scheme (no Base64) and reseller credentials use a custom "reseller" scheme.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: PaySimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaySimple declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PaySimple
provider_slug: paysimple
scheme_count: 2
schemes:
- evidence: Using your PaySimple API username as the user name and API key as the password, use `basic` as the authorization header scheme. This is similar to the standard basic authorization scheme, but there is no Base64 encoding.
  header: Authorization
  how_to_obtain: API username and API key are delivered via encrypted email to the merchant.
  location: header
  name: Merchant Authorization
  type: http-basic
- evidence: If you are issued a reseller API key, input the string `reseller` as the authorization header scheme, followed by a space and the reseller API key.
  header: Authorization
  how_to_obtain: Reseller API key is provided to the reseller by PaySimple.
  location: header
  name: Reseller Authorization
  type: http-basic
slug: paysimple-authentication
source_filename: paysimple-authentication.yml
source_heading: Authentication Profile
source_url: https://documentation.paysimple.com/docs/3d-secure-authentication.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://documentation.paysimple.com/docs/3d-secure-authentication.md\nsources:\n- https://documentation.paysimple.com/docs/3d-secure-authentication.md\n- https://documentation.paysimple.com/reference/authentication-overview.md\n- https://documentation.paysimple.com/reference/authentication-overview\n- https://documentation.paysimple.com/reference/authentication-overview\ndescription: PaySimple requires an Authorization Header for each request. Merchant credentials use a custom \"basic\" scheme (no Base64) and reseller\n  credentials use a custom \"reseller\" scheme.\nschemes:\n- type: http-basic\n  name: Merchant Authorization\n  evidence: Using your PaySimple API username as the user name and API key as the password, use `basic` as the authorization header scheme. This\n    is similar to the standard basic authorization scheme, but there is no Base64 encoding.\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: API username and API key are delivered via encrypted email to the merchant.\n- type: http-basic\n  name: Reseller Authorization\n  evidence: If you are issued a reseller API key, input the string `reseller` as the authorization header scheme, followed by a space and the\n    reseller API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Reseller API key is provided to the reseller by PaySimple.\nnote: Legacy HMAC authorization is no longer recommended and is not described as a current scheme.\ndocs: https://documentation.paysimple.com/docs/3d-secure-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/paysimple/authentication/paysimple-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Billing
- Software-as-a-Service
- Small Business
---
