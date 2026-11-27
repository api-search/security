---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ipogrid-com-articles-api-openapi.yml
  format: yaml
  label: IPOGrid Articles API
  slug: ipogrid-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-articles-api-openapi.yml
- filename: ipogrid-com-companies-api-openapi.yml
  format: yaml
  label: IPOGrid Companies API
  slug: ipogrid-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-companies-api-openapi.yml
- filename: ipogrid-com-filings-api-openapi.yml
  format: yaml
  label: IPOGrid Filings API
  slug: ipogrid-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-filings-api-openapi.yml
- filename: ipogrid-com-news-api-openapi.yml
  format: yaml
  label: IPOGrid News API
  slug: ipogrid-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-news-api-openapi.yml
- filename: ipogrid-com-outcomes-api-openapi.yml
  format: yaml
  label: IPOGrid Outcomes API
  slug: ipogrid-com-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-outcomes-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the page
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: IPOGrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPOGrid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IPOGrid
provider_slug: ipogrid-com
scheme_count: 1
schemes:
- evidence: 'curl -H "Authorization: Bearer $IPOGRID_API_KEY" \ "https://ipogrid.com/api/v1/companies?scope=all&q=spcx&include=latest_terms,classification,consensus"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: ipogrid-com-authentication
source_filename: ipogrid-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ipogrid.com/docs/quickstart
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ipogrid.com/docs/quickstart\nsources:\n- https://ipogrid.com/docs/quickstart\ndescription: Authentication schemes as published on the page\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -H \"Authorization: Bearer $IPOGRID_API_KEY\" \\ \"https://ipogrid.com/api/v1/companies?scope=all&q=spcx&include=latest_terms,classification,consensus\"'\n  location: header\n  header: Authorization\ndocs: https://ipogrid.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/ipogrid-com/authentication/ipogrid-com-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- IPO
- Data
- Research
- Markets
---
