---
api_key_in: []
api_specs:
- filename: open-payments-datastore-query-api-openapi.yml
  format: yaml
  label: CMS Open Payments Datastore Query API
  slug: open-payments-datastore-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-datastore-query-api-openapi.yml
- filename: open-payments-datastore-sql-api-openapi.yml
  format: yaml
  label: CMS Open Payments Datastore SQL API
  slug: open-payments-datastore-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-datastore-sql-api-openapi.yml
- filename: open-payments-download-api-openapi.yml
  format: yaml
  label: CMS Open Payments Download API
  slug: open-payments-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-download-api-openapi.yml
- filename: open-payments-metastore-api-openapi.yml
  format: yaml
  label: CMS Open Payments Metastore API
  slug: open-payments-metastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-metastore-api-openapi.yml
- filename: open-payments-search-api-openapi.yml
  format: yaml
  label: CMS Open Payments Search API
  slug: open-payments-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-search-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: manual
name: Open Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: CMS Open Payments secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CMS Open Payments
provider_slug: open-payments
scheme_count: 1
schemes:
- description: All public read access to the CMS Open Payments data API is open and requires no authentication - no API key, no token, no account. The metastore catalog, search, datastore query, SQL, and download endpoints are all reachable anonymously over HTTPS. This was confirmed live against the API on the review date.
  name: none
  sources:
  - https://openpaymentsdata.cms.gov/about/api
  type: none
slug: open-payments-authentication
source_filename: open-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: manual\nsource: https://openpaymentsdata.cms.gov/about/api\nsummary:\n  types:\n  - none\nschemes:\n- name: none\n  type: none\n  description: >-\n    All public read access to the CMS Open Payments data API is open and requires\n    no authentication - no API key, no token, no account. The metastore catalog,\n    search, datastore query, SQL, and download endpoints are all reachable\n    anonymously over HTTPS. This was confirmed live against the API on the review\n    date.\n  sources:\n  - https://openpaymentsdata.cms.gov/about/api\nnotes: >-\n  The underlying DKAN platform exposes write and content-moderation endpoints that\n  require HTTP Basic Authentication, but those are reserved for CMS data\n  publishers and are not part of the public consumer surface documented here.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/authentication/open-payments-authentication.yml
summary_line: none · 1 scheme
tags:
- Government Data
- Healthcare
- Open Data
- Transparency
- Payments
- Clinical Data
- Physicians
- Open Government
- Public Sector
---
