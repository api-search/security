---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ultralytics-assets-api-openapi.yml
  format: yaml
  label: Ultralytics Assets API
  slug: ultralytics-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-assets-api-openapi.yml
- filename: ultralytics-ultralytics-api-openapi.yml
  format: yaml
  label: Ultralytics Ultralytics API
  slug: ultralytics-ultralytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-ultralytics-api-openapi.yml
- filename: ultralytics-agents-api-openapi.yml
  format: yaml
  label: Ultralytics Agents API
  slug: ultralytics-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-agents-api-openapi.yml
- filename: ultralytics-billing-api-openapi.yml
  format: yaml
  label: Ultralytics Billing API
  slug: ultralytics-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-billing-api-openapi.yml
- filename: ultralytics-datasets-api-openapi.yml
  format: yaml
  label: Ultralytics Datasets API
  slug: ultralytics-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-datasets-api-openapi.yml
- filename: ultralytics-deployments-api-openapi.yml
  format: yaml
  label: Ultralytics Deployments API
  slug: ultralytics-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-deployments-api-openapi.yml
- filename: ultralytics-lifecycle-api-openapi.yml
  format: yaml
  label: Ultralytics Lifecycle API
  slug: ultralytics-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-lifecycle-api-openapi.yml
- filename: ultralytics-storage-integrations-api-openapi.yml
  format: yaml
  label: Ultralytics Storage Integrations API
  slug: ultralytics-storage-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-storage-integrations-api-openapi.yml
- filename: ultralytics-training-api-openapi.yml
  format: yaml
  label: Ultralytics Training API
  slug: ultralytics-training-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-training-api-openapi.yml
- filename: ultralytics-upload-api-openapi.yml
  format: yaml
  label: Ultralytics Upload API
  slug: ultralytics-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ultralytics/openapi/ultralytics-upload-api-openapi.yml
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
source_yaml_url: https://artifacts.apis.io/ultralytics/authentication/ultralytics-authentication.yml
summary_line: 1 scheme
tags:
- Computer Vision
- Artificial Intelligence
- Machine Learning
- Open Source
- Software-as-a-Service
---
