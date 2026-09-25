---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 32 Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: 32 Biosciences secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 32 Biosciences
provider_slug: 32-biosciences
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. The route-discovery document advertises the authorization endpoint at https://32biosciences.com/wp-admin/authorize-application.php. Anonymous read access needs no credential; every write, and the settings and abilities routes, require one.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/32-biosciences-comments-api-openapi.yml
  - openapi/32-biosciences-discovery-api-openapi.yml
  - openapi/32-biosciences-media-api-openapi.yml
  - openapi/32-biosciences-pages-api-openapi.yml
  - openapi/32-biosciences-posts-api-openapi.yml
  - openapi/32-biosciences-settings-api-openapi.yml
  - openapi/32-biosciences-taxonomy-api-openapi.yml
  - openapi/32-biosciences-users-api-openapi.yml
  type: http
slug: 32-biosciences-authentication
source_filename: 32-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/32-biosciences-comments-api-openapi.yml, openapi/32-biosciences-discovery-api-openapi.yml,\n  openapi/32-biosciences-media-api-openapi.yml, openapi/32-biosciences-pages-api-openapi.yml,\n  openapi/32-biosciences-posts-api-openapi.yml, openapi/32-biosciences-settings-api-openapi.yml,\n  openapi/32-biosciences-taxonomy-api-openapi.yml, openapi/32-biosciences-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. The route-discovery document\n    advertises the authorization endpoint at https://32biosciences.com/wp-admin/authorize-application.php.\n    Anonymous read access needs no credential; every write, and the settings and abilities routes,\n    require one.\n  sources:\n  - openapi/32-biosciences-comments-api-openapi.yml\n  - openapi/32-biosciences-discovery-api-openapi.yml\n  - openapi/32-biosciences-media-api-openapi.yml\n\
  \  - openapi/32-biosciences-pages-api-openapi.yml\n  - openapi/32-biosciences-posts-api-openapi.yml\n  - openapi/32-biosciences-settings-api-openapi.yml\n  - openapi/32-biosciences-taxonomy-api-openapi.yml\n  - openapi/32-biosciences-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/32-biosciences/refs/heads/main/authentication/32-biosciences-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Life Sciences
- Gastroenterology
- Microbiome
- Diagnostics
- Therapeutics
- Drug Discovery
- Pharmaceuticals
- Metabolomics
- Healthcare
---
