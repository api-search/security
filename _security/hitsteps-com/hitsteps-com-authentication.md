---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hitsteps-com-openapi-generated.yml
  format: yaml
  label: Hitsteps API
  slug: hitsteps-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hitsteps-com/openapi/_ae-authored/hitsteps-com-openapi-generated.yml
auth_types: []
description: Hitsteps APIs use a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hitsteps Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hitsteps declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hitsteps
provider_slug: hitsteps-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer YOUR_REPORT_API_KEY'
  header: Authorization
  how_to_obtain: Create a key via the Reports API share settings in the Hitsteps dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: hitsteps-com-authentication
source_filename: hitsteps-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hitsteps.com/mac-menubar-setup/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hitsteps.com/mac-menubar-setup/\nsources:\n- https://www.hitsteps.com/mac-menubar-setup/\n- https://www.hitsteps.com/api/reports-api-quickstart.html\n- https://www.hitsteps.com/guide/getting-started/\ndescription: Hitsteps APIs use a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer YOUR_REPORT_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key via the Reports API share settings in the Hitsteps dashboard.\ndocs: https://www.hitsteps.com/mac-menubar-setup/\n"
source_yaml_url: https://artifacts.apis.io/hitsteps-com/authentication/hitsteps-com-authentication.yml
summary_line: 1 scheme
tags:
- Analytics
- Web
- Real-Time
- Statistics
- Marketing
---
