---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: center-for-parent-information-and-resources-account-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Account API
  slug: center-for-parent-information-and-resources-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-account-api-openapi.yml
- filename: center-for-parent-information-and-resources-autocomplete-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Autocomplete API
  slug: center-for-parent-information-and-resources-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-autocomplete-api-openapi.yml
- filename: center-for-parent-information-and-resources-categories-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Categories API
  slug: center-for-parent-information-and-resources-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-categories-api-openapi.yml
- filename: center-for-parent-information-and-resources-countries-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Countries API
  slug: center-for-parent-information-and-resources-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-countries-api-openapi.yml
- filename: center-for-parent-information-and-resources-discovery-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Discovery API
  slug: center-for-parent-information-and-resources-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-discovery-api-openapi.yml
- filename: center-for-parent-information-and-resources-entries-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Entries API
  slug: center-for-parent-information-and-resources-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-entries-api-openapi.yml
- filename: center-for-parent-information-and-resources-geometry-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Geometry API
  slug: center-for-parent-information-and-resources-geometry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-geometry-api-openapi.yml
- filename: center-for-parent-information-and-resources-metadata-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Metadata API
  slug: center-for-parent-information-and-resources-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-metadata-api-openapi.yml
- filename: center-for-parent-information-and-resources-regions-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources Regions API
  slug: center-for-parent-information-and-resources-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-regions-api-openapi.yml
- filename: center-for-parent-information-and-resources-seo-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources SEO API
  slug: center-for-parent-information-and-resources-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-seo-api-openapi.yml
- filename: center-for-parent-information-and-resources-o-embed-api-openapi.yml
  format: yaml
  label: Center for Parent Information and Resources o Embed API
  slug: center-for-parent-information-and-resources-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-o-embed-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Center For Parent Information And Resources Authentication
name_suffix: Authentication
oauth_flows: []
overview: Center for Parent Information and Resources secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Center for Parent Information and Resources
provider_slug: center-for-parent-information-and-resources
scheme_count: 1
schemes:
- description: WordPress cookie authentication paired with an `X-WP-Nonce` header.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/center-for-parent-information-and-resources-oembed-api-openapi.yml
  - openapi/center-for-parent-information-and-resources-parent-center-directory-api-openapi.yml
  type: apiKey
slug: center-for-parent-information-and-resources-authentication
source_filename: center-for-parent-information-and-resources-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/center-for-parent-information-and-resources-oembed-api-openapi.yml, openapi/center-for-parent-information-and-resources-parent-center-directory-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication paired with an `X-WP-Nonce` header.\n  sources:\n  - openapi/center-for-parent-information-and-resources-oembed-api-openapi.yml\n  - openapi/center-for-parent-information-and-resources-parent-center-directory-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/authentication/center-for-parent-information-and-resources-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Disability
- Education
- Families
- Federal-Government
- Parent Centers
- Parent Training
- Parents
- Special Needs
---
