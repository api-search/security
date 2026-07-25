---
api_key_in: []
api_specs:
- filename: apache-nutch-admin-api-openapi.yml
  format: yaml
  label: Apache Nutch Admin API
  slug: apache-nutch-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-admin-api-openapi.yml
- filename: apache-nutch-configuration-api-openapi.yml
  format: yaml
  label: Apache Nutch Configuration API
  slug: apache-nutch-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-configuration-api-openapi.yml
- filename: apache-nutch-database-api-openapi.yml
  format: yaml
  label: Apache Nutch Database API
  slug: apache-nutch-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-database-api-openapi.yml
- filename: apache-nutch-job-api-openapi.yml
  format: yaml
  label: Apache Nutch Job API
  slug: apache-nutch-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-job-api-openapi.yml
- filename: apache-nutch-reader-api-openapi.yml
  format: yaml
  label: Apache Nutch Reader API
  slug: apache-nutch-reader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-reader-api-openapi.yml
- filename: apache-nutch-seed-api-openapi.yml
  format: yaml
  label: Apache Nutch Seed API
  slug: apache-nutch-seed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-seed-api-openapi.yml
- filename: apache-nutch-services-api-openapi.yml
  format: yaml
  label: Apache Nutch Services API
  slug: apache-nutch-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Nutch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Nutch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Nutch
provider_slug: apache-nutch
scheme_count: 1
schemes:
- description: HTTP Basic Authentication.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-nutch-openapi.yaml
  type: http
slug: apache-nutch-authentication
source_filename: apache-nutch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-nutch-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication.\n  sources:\n  - openapi/apache-nutch-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/authentication/apache-nutch-authentication.yml
summary_line: http · 1 scheme
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
---
