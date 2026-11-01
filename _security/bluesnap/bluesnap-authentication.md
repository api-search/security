---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for BlueSnap APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bluesnap Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueSnap declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BlueSnap
provider_slug: bluesnap
scheme_count: 1
schemes:
- evidence: 'Every API request must be authenticated using a HTTP Basic Authentication header, as follows: `authorization: Basic {Base64 encoding of ''username:password''}`'
  header: authorization
  how_to_obtain: The username and password can be found in the Merchant Portal, under Settings > API Settings.
  location: header
  name: Basic
  type: http-basic
slug: bluesnap-authentication
source_filename: bluesnap-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.bluesnap.com/reference/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.bluesnap.com/reference/authentication.md\nsources:\n- https://developers.bluesnap.com/reference/authentication.md\n- https://developers.bluesnap.com/reference/api-credentials.md\ndescription: Authentication schemes for BlueSnap APIs\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: 'Every API request must be authenticated using a HTTP Basic Authentication header, as follows: `authorization: Basic {Base64 encoding\n    of ''username:password''}`'\n  location: header\n  header: authorization\n  how_to_obtain: The username and password can be found in the Merchant Portal, under Settings > API Settings.\nnote: Only 1 space is allowed after the \"Basic\" prefix and before you add the Base64 encoding.\ndocs: https://developers.bluesnap.com/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/bluesnap/authentication/bluesnap-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- FinTech
- API
- GlobalPayments
---
