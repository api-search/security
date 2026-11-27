---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gimmetext-com-jobs-api-openapi.yml
  format: yaml
  label: GimmeText Jobs API
  slug: gimmetext-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-jobs-api-openapi.yml
- filename: gimmetext-com-uploads-api-openapi.yml
  format: yaml
  label: GimmeText Uploads API
  slug: gimmetext-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-uploads-api-openapi.yml
- filename: gimmetext-com-usage-api-openapi.yml
  format: yaml
  label: GimmeText Usage API
  slug: gimmetext-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-usage-api-openapi.yml
auth_types: []
description: Authentication schemes for GimmeText API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GimmeText Authentication
name_suffix: Authentication
oauth_flows: []
overview: GimmeText declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GimmeText
provider_slug: gimmetext-com
scheme_count: 1
schemes:
- evidence: 'Every request needs `Authorization: Bearer gt_live_XXXX`.'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: gimmetext-com-authentication
source_filename: gimmetext-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gimmetext.com/docs/api.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gimmetext.com/docs/api.md\nsources:\n- https://gimmetext.com/docs/api.md\ndescription: Authentication schemes for GimmeText API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request needs `Authorization: Bearer gt_live_XXXX`.'\n  location: header\n  header: Authorization\ndocs: https://gimmetext.com/docs/api.md\n"
source_yaml_url: https://artifacts.apis.io/gimmetext-com/authentication/gimmetext-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Transcription
- Audio
- Video
- Privacy
- Software-as-a-Service
---
