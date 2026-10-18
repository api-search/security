---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ultralytics-assets-api-openapi.yml
  format: yaml
  label: Ultralytics Assets API
  slug: ultralytics-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultralytics/refs/heads/main/openapi/ultralytics-assets-api-openapi.yml
- filename: ultralytics-ultralytics-api-openapi.yml
  format: yaml
  label: Ultralytics Ultralytics API
  slug: ultralytics-ultralytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultralytics/refs/heads/main/openapi/ultralytics-ultralytics-api-openapi.yml
auth_types: []
description: Ultralytics API authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ultralytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ultralytics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ultralytics
provider_slug: ultralytics
scheme_count: 1
schemes:
- evidence: "Include the key in API requests:\n\n```bash\ncurl -H \"Authorization: Bearer YOUR_API_KEY\" \\\n  https://platform.ultralytics.com/api/...\n```"
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
slug: ultralytics-authentication
source_filename: ultralytics-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ultralytics.com/platform/account/api-keys.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ultralytics.com/platform/account/api-keys.md\nsources:\n- https://docs.ultralytics.com/platform/account/api-keys.md\n- https://docs.ultralytics.com/quickstart.md\n- https://docs.ultralytics.com/guides/conda-quickstart.md\n- https://docs.ultralytics.com/guides/docker-quickstart.md\ndescription: Ultralytics API authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: \"Include the key in API requests:\\n\\n```bash\\ncurl -H \\\"Authorization: Bearer YOUR_API_KEY\\\" \\\\\\n  https://platform.ultralytics.com/api/...\\n\\\n    ```\"\n  location: header\n  header: Authorization\nnote: No OAuth2, API key query, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.ultralytics.com/platform/account/api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultralytics/refs/heads/main/authentication/ultralytics-authentication.yml
summary_line: 1 scheme
tags:
- Computer Vision
- Artificial Intelligence
- Machine Learning
- Open Source
- Software-as-a-Service
---
