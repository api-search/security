---
api_key_in: []
api_specs:
- filename: apache-solr-schema-api-openapi.yml
  format: yaml
  label: Apache Solr Schema API
  slug: apache-solr-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-schema-api-openapi.yml
- filename: apache-solr-collections-api-openapi.yml
  format: yaml
  label: Apache Solr Collections API
  slug: apache-solr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-collections-api-openapi.yml
- filename: apache-solr-cluster-api-openapi.yml
  format: yaml
  label: Apache Solr Cluster API
  slug: apache-solr-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-cluster-api-openapi.yml
- filename: apache-solr-collections-api-openapi.yml
  format: yaml
  label: Apache Solr Collections API
  slug: apache-solr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-collections-api-openapi.yml
- filename: apache-solr-query-api-openapi.yml
  format: yaml
  label: Apache Solr Query API
  slug: apache-solr-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-query-api-openapi.yml
- filename: apache-solr-schema-api-openapi.yml
  format: yaml
  label: Apache Solr Schema API
  slug: apache-solr-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-schema-api-openapi.yml
- filename: apache-solr-update-api-openapi.yml
  format: yaml
  label: Apache Solr Update API
  slug: apache-solr-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/openapi/apache-solr-update-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Solr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Solr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Solr
provider_slug: apache-solr
scheme_count: 1
schemes:
- description: Enabled when Solr's BasicAuthPlugin is configured
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-solr-openapi.yml
  type: http
slug: apache-solr-authentication
source_filename: apache-solr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-solr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Enabled when Solr's BasicAuthPlugin is configured\n  sources:\n  - openapi/apache-solr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-solr/refs/heads/main/authentication/apache-solr-authentication.yml
summary_line: http · 1 scheme
tags:
- Enterprise Search
- Full-Text Search
- Lucene
- Search
- SolrCloud
- Open Source
- Java
---
