---
anonymous_access: false
api_key_in: []
api_specs:
- filename: generect-com-1-auth-api-openapi.yml
  format: yaml
  label: Generect 1. Auth API
  slug: generect-com-1-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-1-auth-api-openapi.yml
- filename: generect-com-10-phone-api-openapi.yml
  format: yaml
  label: Generect 10. Phone API
  slug: generect-com-10-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-10-phone-api-openapi.yml
- filename: generect-com-11-webhooks-api-openapi.yml
  format: yaml
  label: Generect 11. Webhooks API
  slug: generect-com-11-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-11-webhooks-api-openapi.yml
- filename: generect-com-2-transactions-api-openapi.yml
  format: yaml
  label: Generect 2. Transactions API
  slug: generect-com-2-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-2-transactions-api-openapi.yml
- filename: generect-com-3-leads-api-openapi.yml
  format: yaml
  label: Generect 3. Leads API
  slug: generect-com-3-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-3-leads-api-openapi.yml
- filename: generect-com-4-companies-api-openapi.yml
  format: yaml
  label: Generect 4. Companies API
  slug: generect-com-4-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-4-companies-api-openapi.yml
- filename: generect-com-5-preview-api-openapi.yml
  format: yaml
  label: Generect 5. Preview API
  slug: generect-com-5-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-5-preview-api-openapi.yml
- filename: generect-com-6-enrich-api-openapi.yml
  format: yaml
  label: Generect 6. Enrich API
  slug: generect-com-6-enrich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-6-enrich-api-openapi.yml
- filename: generect-com-7-email-api-openapi.yml
  format: yaml
  label: Generect 7. Email API
  slug: generect-com-7-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-7-email-api-openapi.yml
- filename: generect-com-8-accounts-api-openapi.yml
  format: yaml
  label: Generect 8. Accounts API
  slug: generect-com-8-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-8-accounts-api-openapi.yml
- filename: generect-com-9-search-api-openapi.yml
  format: yaml
  label: Generect 9. Search API
  slug: generect-com-9-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-9-search-api-openapi.yml
- filename: generect-com-auth-api-openapi.yml
  format: yaml
  label: Generect Auth API
  slug: generect-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-auth-api-openapi.yml
- filename: generect-com-linked-in-api-openapi.yml
  format: yaml
  label: Generect Linked In API
  slug: generect-com-linked-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/generect-com/openapi/generect-com-linked-in-api-openapi.yml
auth_types: []
description: Authentication via API token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Generect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Generect declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Generect
provider_slug: generect-com
scheme_count: 1
schemes:
- evidence: To authenticate requests, include your API token in the `Authorization` header.
  header: Authorization
  how_to_obtain: You can get your API token from the Generect app settings.
  location: header
  name: apiKey
  type: apiKey
slug: generect-com-authentication
source_filename: generect-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.generect.com/api-reference/authentication.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.generect.com/api-reference/authentication.md\nsources:\n- https://docs.generect.com/api-reference/authentication.md\n- https://docs.generect.com/api-reference/endpoint/accounts/get-account-token-analytics.md\n- https://docs.generect.com/api-reference/quickstart.md\n- https://docs.generect.com/integrations/mcp/quick-start.md\ndescription: Authentication via API token\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: To authenticate requests, include your API token in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: You can get your API token from the Generect app settings.\ndocs: https://docs.generect.com/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/generect-com/authentication/generect-com-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Lead Generation
- Real-Time Data
- Software-as-a-Service
---
