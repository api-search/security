---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for EarthScope APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Earthscope Consortium Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: EarthScope Consortium, Inc. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EarthScope Consortium, Inc.
provider_slug: earthscope-consortium-inc
scheme_count: 1
schemes:
- authorize_url: https://login.earthscope.org/activate?user_code=ABCD-EFGH
  evidence: 'If the browser does not open or you wish to use a different device to authorize this request, open the following URL: https://login.earthscope.org/activate?user_code=ABCD-EFGH'
  flows:
  - device_code
  how_to_obtain: Use the `es login` CLI command which opens the SSO authorization page; if it does not open, copy the provided URL into a browser.
  name: EarthScope OAuth2
  type: oauth2
slug: earthscope-consortium-inc-authentication
source_filename: earthscope-consortium-inc-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.earthscope.org/cli/authentication
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.earthscope.org/cli/authentication\nsources:\n- https://docs.earthscope.org/cli/authentication\n- https://docs.earthscope.org/sdk/authentication\n- https://docs.earthscope.org/geolab/getting-started\n- https://docs.earthscope.org/geolab/getting-started/access\ndescription: Authentication schemes for EarthScope APIs\nschemes:\n- type: oauth2\n  name: EarthScope OAuth2\n  evidence: 'If the browser does not open or you wish to use a different device to authorize this request, open the following URL: https://login.earthscope.org/activate?user_code=ABCD-EFGH'\n  flows:\n  - device_code\n  authorize_url: https://login.earthscope.org/activate?user_code=ABCD-EFGH\n  how_to_obtain: Use the `es login` CLI command which opens the SSO authorization page; if it does not open, copy the provided URL into a browser.\ndocs: https://docs.earthscope.org/cli/authentication\n"
source_yaml_url: https://artifacts.apis.io/earthscope-consortium-inc/authentication/earthscope-consortium-inc-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Geophysics
- Research
- Education
- NSF
---
