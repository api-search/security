---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aistrail Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIS Trail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AIS Trail
provider_slug: aistrail-com
scheme_count: 1
schemes:
- evidence: 'Send the key in a header on every request: Authorization: Bearer ap_live_YOUR_KEY'
  header: Authorization
  how_to_obtain: Create an API key on the API keys page of your dashboard; the key is prefixed with ap_live_ and 32 characters.
  location: header
  name: Bearer
  type: http-bearer
slug: aistrail-com-authentication
source_filename: aistrail-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aistrail.com/docs/quickstart/
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aistrail.com/docs/quickstart/\nsources:\n- https://aistrail.com/docs/quickstart/\n- https://aistrail.com/docs/quickstart/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the key in a header on every request: Authorization: Bearer ap_live_YOUR_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the API keys page of your dashboard; the key is prefixed with ap_live_ and 32 characters.\nnote: The API does not accept the key in the URL.\ndocs: https://aistrail.com/docs/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/aistrail-com/authentication/aistrail-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Maritime
- AIS
- Data
- Real-Time
---
