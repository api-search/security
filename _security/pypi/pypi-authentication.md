---
api_key_in: []
api_specs:
- filename: pypi-json-api-openapi.yml
  format: yaml
  label: PyPI JSON API
  slug: json
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-json-api-openapi.yml
- filename: pypi-index-api-openapi.yml
  format: yaml
  label: PyPI Index API
  slug: index
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-index-api-openapi.yml
- filename: pypi-integrity-api-openapi.yml
  format: yaml
  label: PyPI Integrity API
  slug: integrity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-integrity-api-openapi.yml
- filename: pypi-upload-api-openapi.yml
  format: yaml
  label: PyPI Upload API
  slug: upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-upload-api-openapi.yml
- filename: pypi-stats-api-openapi.yml
  format: yaml
  label: PyPI Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-stats-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pypi Authentication
name_suffix: Authentication
oauth_flows: []
overview: PyPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PyPI
provider_slug: pypi
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using __token__ as the username and a PyPI API token as the password. Trusted Publishers receive short-lived tokens through OpenID Connect that are used in the same manner.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pypi-upload-api-openapi.yml
  type: http
slug: pypi-authentication
source_filename: pypi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pypi-upload-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using __token__ as the username and a PyPI API token\n    as the password. Trusted Publishers receive short-lived tokens through OpenID Connect that\n    are used in the same manner.\n  sources:\n  - openapi/pypi-upload-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/authentication/pypi-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Open Source
- Package Management
- Packages
- Python
---
