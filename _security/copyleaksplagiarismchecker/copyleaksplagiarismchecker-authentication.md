---
anonymous_access: false
api_key_in: []
api_specs:
- filename: copyleaksplagiarismchecker-ai-image-detector-async-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Ai Image Detector Async API
  slug: copyleaksplagiarismchecker-ai-image-detector-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-ai-image-detector-async-api-openapi.yml
- filename: copyleaksplagiarismchecker-ai-video-detector-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Ai Video Detector API
  slug: copyleaksplagiarismchecker-ai-video-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-ai-video-detector-api-openapi.yml
- filename: copyleaksplagiarismchecker-downloads-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Downloads API
  slug: copyleaksplagiarismchecker-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-downloads-api-openapi.yml
- filename: copyleaksplagiarismchecker-my-scan-123-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker My Scan 123 API
  slug: copyleaksplagiarismchecker-my-scan-123-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-my-scan-123-api-openapi.yml
- filename: copyleaksplagiarismchecker-repositories-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Repositories API
  slug: copyleaksplagiarismchecker-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-repositories-api-openapi.yml
- filename: copyleaksplagiarismchecker-scans-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Scans API
  slug: copyleaksplagiarismchecker-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-scans-api-openapi.yml
- filename: copyleaksplagiarismchecker-writer-detector-api-openapi.yml
  format: yaml
  label: Copyleaksplagiarismchecker Writer Detector API
  slug: copyleaksplagiarismchecker-writer-detector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/openapi/copyleaksplagiarismchecker-writer-detector-api-openapi.yml
auth_types: []
description: 'Authentication uses a two‑part model. First, a POST to the login endpoint with an email and API key in the JSON body returns an access_token. Subsequent API calls require the token in an Authorization: Bearer header.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Copyleaksplagiarismchecker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copyleaksplagiarismchecker declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Copyleaksplagiarismchecker
provider_slug: copyleaksplagiarismchecker
scheme_count: 1
schemes:
- evidence: This token must be sent with every subsequent API request in the Authorization header.
  header: Authorization
  how_to_obtain: Use the access_token returned from the login endpoint.
  location: header
  name: Access token
  type: http-bearer
slug: copyleaksplagiarismchecker-authentication
source_filename: copyleaksplagiarismchecker-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.copyleaks.com/using-the-apis/authentication
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.copyleaks.com/using-the-apis/authentication\nsources:\n- https://docs.copyleaks.com/using-the-apis/authentication\n- https://docs.copyleaks.com/get-started/quickstart\n- https://docs.copyleaks.com/resources/sdks/python\n- https://docs.copyleaks.com/resources/sdks/javascript\ndescription: 'Authentication uses a two‑part model. First, a POST to the login endpoint with an email and API key in the JSON body returns an\n  access_token. Subsequent API calls require the token in an Authorization: Bearer header.'\nschemes:\n- type: http-bearer\n  name: Access token\n  evidence: This token must be sent with every subsequent API request in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Use the access_token returned from the login endpoint.\nnote: No OAuth flows, apiKey header, or other standard schemes are documented. 1 extracted row(s)\
  \ were dropped because their quote was not on\n  the page.\ndocs: https://docs.copyleaks.com/using-the-apis/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copyleaksplagiarismchecker/refs/heads/main/authentication/copyleaksplagiarismchecker-authentication.yml
summary_line: 1 scheme
tags:
- AI Detection
- Plagiarism Checker
- Content Integrity
- Education
- Enterprise
- Media Publishing
- API Integration
---
