---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: center-for-parent-information-and-resources-parent-center-directory-api-openapi.yml
  format: yaml
  label: CPIR Parent Center Directory API
  slug: cpir-parent-center-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-parent-center-directory-api-openapi.yml
- filename: center-for-parent-information-and-resources-geography-reference-api-openapi.yml
  format: yaml
  label: CPIR Geography Reference API
  slug: cpir-geography-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-geography-reference-api-openapi.yml
- filename: center-for-parent-information-and-resources-oembed-api-openapi.yml
  format: yaml
  label: CPIR oEmbed API
  slug: cpir-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-oembed-api-openapi.yml
- filename: center-for-parent-information-and-resources-site-metadata-api-openapi.yml
  format: yaml
  label: CPIR Site Metadata API
  slug: cpir-site-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/center-for-parent-information-and-resources/refs/heads/main/openapi/center-for-parent-information-and-resources-site-metadata-api-openapi.yml
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
