---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: abyssale-com-auth-api-openapi.yml
  format: yaml
  label: Abyssale Auth API
  slug: abyssale-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-auth-api-openapi.yml
- filename: abyssale-com-credits-api-openapi.yml
  format: yaml
  label: Abyssale Credits API
  slug: abyssale-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-credits-api-openapi.yml
- filename: abyssale-com-design-duplication-requests-api-openapi.yml
  format: yaml
  label: Abyssale Design Duplication Requests API
  slug: abyssale-com-design-duplication-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-design-duplication-requests-api-openapi.yml
- filename: abyssale-com-designs-api-openapi.yml
  format: yaml
  label: Abyssale Designs API
  slug: abyssale-com-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-designs-api-openapi.yml
- filename: abyssale-com-examples-api-openapi.yml
  format: yaml
  label: Abyssale Examples API
  slug: abyssale-com-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-examples-api-openapi.yml
- filename: abyssale-com-export-abyssale-api-openapi.yml
  format: yaml
  label: Abyssale Export Abyssale API
  slug: abyssale-com-export-abyssale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-export-abyssale-api-openapi.yml
- filename: abyssale-com-fonts-api-openapi.yml
  format: yaml
  label: Abyssale Fonts API
  slug: abyssale-com-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-fonts-api-openapi.yml
- filename: abyssale-com-images-api-openapi.yml
  format: yaml
  label: Abyssale Images API
  slug: abyssale-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-images-api-openapi.yml
- filename: abyssale-com-projects-api-openapi.yml
  format: yaml
  label: Abyssale Projects API
  slug: abyssale-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-projects-api-openapi.yml
- filename: abyssale-com-workspace-template-categories-api-openapi.yml
  format: yaml
  label: Abyssale Workspace Template Categories API
  slug: abyssale-com-workspace-template-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-workspace-template-categories-api-openapi.yml
- filename: abyssale-com-workspace-templates-api-openapi.yml
  format: yaml
  label: Abyssale Workspace Templates API
  slug: abyssale-com-workspace-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-workspace-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Abyssale Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abyssale secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abyssale
provider_slug: abyssale-com
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/abyssale-com-openapi-generated.yml
  type: apiKey
slug: abyssale-com-authentication
source_filename: abyssale-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/abyssale-com-openapi-generated.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/abyssale-com-openapi-generated.yml\n"
source_yaml_url: https://artifacts.apis.io/abyssale-com/authentication/abyssale-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Creative Automation
- Marketing
- Agencies
- Visual-Production
- Software-as-a-Service
---
