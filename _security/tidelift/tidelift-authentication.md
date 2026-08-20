---
api_key_in: []
api_specs:
- filename: tidelift-alignments-api-openapi.yml
  format: yaml
  label: Tidelift Alignments API
  slug: tidelift-alignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-alignments-api-openapi.yml
- filename: tidelift-attestations-api-openapi.yml
  format: yaml
  label: Tidelift Attestations API
  slug: tidelift-attestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-attestations-api-openapi.yml
- filename: tidelift-authentication-api-openapi.yml
  format: yaml
  label: Tidelift Authentication API
  slug: tidelift-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-authentication-api-openapi.yml
- filename: tidelift-basic-examples-api-openapi.yml
  format: yaml
  label: Tidelift Basic Examples API
  slug: tidelift-basic-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-basic-examples-api-openapi.yml
- filename: tidelift-catalog-releases-api-openapi.yml
  format: yaml
  label: Tidelift Catalog Releases API
  slug: tidelift-catalog-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-catalog-releases-api-openapi.yml
- filename: tidelift-catalogs-api-openapi.yml
  format: yaml
  label: Tidelift Catalogs API
  slug: tidelift-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-catalogs-api-openapi.yml
- filename: tidelift-catalogstandards-api-openapi.yml
  format: yaml
  label: Tidelift CatalogStandards API
  slug: tidelift-catalogstandards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-catalogstandards-api-openapi.yml
- filename: tidelift-groups-api-openapi.yml
  format: yaml
  label: Tidelift Groups API
  slug: tidelift-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-groups-api-openapi.yml
- filename: tidelift-licenses-api-openapi.yml
  format: yaml
  label: Tidelift Licenses API
  slug: tidelift-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-licenses-api-openapi.yml
- filename: tidelift-packages-api-openapi.yml
  format: yaml
  label: Tidelift Packages API
  slug: tidelift-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-packages-api-openapi.yml
- filename: tidelift-projects-api-openapi.yml
  format: yaml
  label: Tidelift Projects API
  slug: tidelift-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-projects-api-openapi.yml
- filename: tidelift-releases-api-openapi.yml
  format: yaml
  label: Tidelift Releases API
  slug: tidelift-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-releases-api-openapi.yml
- filename: tidelift-reports-api-openapi.yml
  format: yaml
  label: Tidelift Reports API
  slug: tidelift-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-reports-api-openapi.yml
- filename: tidelift-users-api-openapi.yml
  format: yaml
  label: Tidelift Users API
  slug: tidelift-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-users-api-openapi.yml
- filename: tidelift-vulnerabilities-api-openapi.yml
  format: yaml
  label: Tidelift Vulnerabilities API
  slug: tidelift-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/openapi/tidelift-vulnerabilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tidelift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tidelift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tidelift
provider_slug: tidelift
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tidelift-subscriber-api-openapi-original.json
  type: http
slug: tidelift-authentication
source_filename: tidelift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tidelift-subscriber-api-openapi-original.json\ndocs: https://docs.tidelift.com/article/79-api-authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  key_types:\n  - user\n  - project\n  - organization\n  note: >-\n    A Tidelift API key is required for all External API endpoints, passed as a Bearer token\n    in the Authorization header. The security requirement declares three key scopes\n    (user, project, organization); each path documents which key type it accepts.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tidelift-subscriber-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidelift/refs/heads/main/authentication/tidelift-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Open-Source
- Software Supply Chain
- Dependency Management
- Application Security
- SBOM
- License Compliance
- Vulnerability Management
- Developer Tools
---
