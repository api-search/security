---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lenz-io-account-api-openapi.yml
  format: yaml
  label: lenz-io Account API
  slug: lenz-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-account-api-openapi.yml
- filename: lenz-io-ask-api-openapi.yml
  format: yaml
  label: lenz-io Ask API
  slug: lenz-io-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-ask-api-openapi.yml
- filename: lenz-io-assess-api-openapi.yml
  format: yaml
  label: lenz-io Assess API
  slug: lenz-io-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-assess-api-openapi.yml
- filename: lenz-io-citecheck-api-openapi.yml
  format: yaml
  label: lenz-io Citecheck API
  slug: lenz-io-citecheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-citecheck-api-openapi.yml
- filename: lenz-io-discovery-api-openapi.yml
  format: yaml
  label: lenz-io Discovery API
  slug: lenz-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-discovery-api-openapi.yml
- filename: lenz-io-extract-api-openapi.yml
  format: yaml
  label: lenz-io Extract API
  slug: lenz-io-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-extract-api-openapi.yml
- filename: lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
  format: yaml
  label: lenz-io Lenz — AI Fact Checking API
  slug: lenz-io-lenz-ai-fact-checking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
- filename: lenz-io-library-api-openapi.yml
  format: yaml
  label: lenz-io Library API
  slug: lenz-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-library-api-openapi.yml
- filename: lenz-io-review-api-openapi.yml
  format: yaml
  label: lenz-io Review API
  slug: lenz-io-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-review-api-openapi.yml
- filename: lenz-io-verifications-api-openapi.yml
  format: yaml
  label: lenz-io Verifications API
  slug: lenz-io-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verifications-api-openapi.yml
- filename: lenz-io-verify-api-openapi.yml
  format: yaml
  label: lenz-io Verify API
  slug: lenz-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verify-api-openapi.yml
auth_types: []
description: Authentication schemes for Lenz API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lenz Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: lenz-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: lenz-io
provider_slug: lenz-io
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://lenz.io/api/v1/assess \ -H "Authorization: Bearer $LENZ_API_KEY" \ -H "X-Lenz-API-Version: 2026-10-11" \ -H "Content-Type: application/json" \ -d ''{"claim": "The Great Wall of China is visible from space."}'''
  header: Authorization
  how_to_obtain: Sign up and generate a key at /api-credentials ; it is shown once, so copy it somewhere safe.
  location: header
  name: Bearer
  type: http-bearer
slug: lenz-io-authentication
source_filename: lenz-io-authentication.yml
source_heading: Authentication Profile
source_url: https://lenz.io/docs/quickstart
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lenz.io/docs/quickstart\nsources:\n- https://lenz.io/docs/quickstart\ndescription: Authentication schemes for Lenz API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -X POST https://lenz.io/api/v1/assess \\ -H \"Authorization: Bearer $LENZ_API_KEY\" \\ -H \"X-Lenz-API-Version: 2026-10-11\" \\ -H\n    \"Content-Type: application/json\" \\ -d ''{\"claim\": \"The Great Wall of China is visible from space.\"}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up and generate a key at /api-credentials ; it is shown once, so copy it somewhere safe.\ndocs: https://lenz.io/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/lenz-io/authentication/lenz-io-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Fact-Checking
- Enterprise
- API
- Audit
---
