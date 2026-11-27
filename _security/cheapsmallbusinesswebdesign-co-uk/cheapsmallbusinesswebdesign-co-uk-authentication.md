---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cheapsmallbusinesswebdesign-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Cheap Small Business Web Design Enquiry API
  slug: cheapsmallbusinesswebdesign-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapsmallbusinesswebdesign-co-uk/openapi/cheapsmallbusinesswebdesign-co-uk-enquiry-api-openapi.yml
- filename: cheapsmallbusinesswebdesign-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Cheap Small Business Web Design MCP API
  slug: cheapsmallbusinesswebdesign-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cheapsmallbusinesswebdesign-co-uk/openapi/cheapsmallbusinesswebdesign-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cheap Small Business Web Design Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cheap Small Business Web Design secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cheap Small Business Web Design
provider_slug: cheapsmallbusinesswebdesign-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cheapsmallbusinesswebdesign-co-uk-openapi.yml
  type: http
slug: cheapsmallbusinesswebdesign-co-uk-authentication
source_filename: cheapsmallbusinesswebdesign-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/cheapsmallbusinesswebdesign-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cheapsmallbusinesswebdesign-co-uk-openapi.yml\ndocs: https://cheapsmallbusinesswebdesign.co.uk/mcp\nnote: 'The provider MCP card (GET https://cheapsmallbusinesswebdesign.co.uk/mcp, 200, 2026-11-03) declares \"auth\": \"none\" for the MCP endpoint; the OpenAPI declares an optional bearer access key (emk_...) that raises the free-tier ceiling. No top-level security requirement is set in the spec, so calls are unauthenticated by default.'\n"
source_yaml_url: https://artifacts.apis.io/cheapsmallbusinesswebdesign-co-uk/authentication/cheapsmallbusinesswebdesign-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web Design
- Small Business
- United Kingdom
- Pricing Data
- Websites
---
