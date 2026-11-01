---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dittowords-activity-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Activity API
  slug: dittowords-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-activity-api-openapi.yml
- filename: dittowords-component-folders-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Component Folders API
  slug: dittowords-component-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-component-folders-api-openapi.yml
- filename: dittowords-components-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Components API
  slug: dittowords-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-components-api-openapi.yml
- filename: dittowords-components-folders-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Components Folders API
  slug: dittowords-components-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-components-folders-api-openapi.yml
- filename: dittowords-project-blocks-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Project Blocks API
  slug: dittowords-project-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-project-blocks-api-openapi.yml
- filename: dittowords-projects-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Projects API
  slug: dittowords-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-projects-api-openapi.yml
- filename: dittowords-statuses-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Statuses API
  slug: dittowords-statuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-statuses-api-openapi.yml
- filename: dittowords-text-items-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Text Items API
  slug: dittowords-text-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-text-items-api-openapi.yml
- filename: dittowords-variables-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Variables API
  slug: dittowords-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-variables-api-openapi.yml
- filename: dittowords-variants-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Variants API
  slug: dittowords-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-variants-api-openapi.yml
- filename: dittowords-styleguides-api-openapi.yml
  format: yaml
  label: Ditto (dittowords.com) Styleguides API
  slug: dittowords-styleguides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dittowords/openapi/dittowords-styleguides-api-openapi.yml
auth_types: []
description: Authentication schemes for Ditto API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dittowords Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ditto (dittowords.com) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ditto (dittowords.com)
provider_slug: dittowords
scheme_count: 2
schemes:
- evidence: 'Pass the key in the `Authorization` header with the `token` scheme:'
  header: Authorization
  how_to_obtain: Create an API key in Ditto under Developers → API keys.
  location: header
  name: API key (current API)
  type: other
- evidence: 'Authorize requests to the Ditto API by passing an API key in an `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate an API key via the Developer Integrations page.
  location: header
  name: API key (legacy API)
  type: other
slug: dittowords-authentication
source_filename: dittowords-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.dittowords.com/cli-reference/authentication.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.dittowords.com/cli-reference/authentication.md\nsources:\n- https://developer.dittowords.com/cli-reference/authentication.md\n- https://developer.dittowords.com/api-reference/authentication.md\n- https://developer.dittowords.com/legacy/api-reference-legacy/authentication.md\n- https://developer.dittowords.com/legacy/cli-reference-legacy/authentication.md\ndescription: Authentication schemes for Ditto API\nschemes:\n- type: other\n  name: API key (current API)\n  evidence: 'Pass the key in the `Authorization` header with the `token` scheme:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Ditto under Developers → API keys.\n- type: other\n  name: API key (legacy API)\n  evidence: 'Authorize requests to the Ditto API by passing an API key in an `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Generate an API key via the Developer Integrations page.\ndocs: https://developer.dittowords.com/cli-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/dittowords/authentication/dittowords-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Content
- Localization
- SaaS
---
