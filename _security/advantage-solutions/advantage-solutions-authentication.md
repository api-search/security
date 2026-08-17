---
api_key_in: []
api_specs:
- filename: advantage-solutions-youradv-content-openapi.yml
  format: yaml
  label: Advantage Solutions Corporate Content API (WordPress REST)
  slug: youradv-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/openapi/advantage-solutions-youradv-content-openapi.yml
- filename: advantage-solutions-mrktblog-content-openapi.yml
  format: yaml
  label: MRKT Blog Content API (WordPress REST)
  slug: mrktblog-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/openapi/advantage-solutions-mrktblog-content-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Advantage Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advantage Solutions secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Advantage Solutions
provider_slug: advantage-solutions
scheme_count: 1
schemes:
- description: WordPress Application Passwords (HTTP Basic). The discovery document advertises the authorization endpoint at https://mrktblog.com/wp-admin/authorize-application.php. Read operations on published content are anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/advantage-solutions-mrktblog-content-openapi.yml
  - openapi/advantage-solutions-youradv-content-openapi.yml
  type: http
slug: advantage-solutions-authentication
source_filename: advantage-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/advantage-solutions-mrktblog-content-openapi.yml, openapi/advantage-solutions-youradv-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (HTTP Basic). The discovery document advertises\n    the authorization endpoint at https://mrktblog.com/wp-admin/authorize-application.php. Read\n    operations on published content are anonymous.\n  sources:\n  - openapi/advantage-solutions-mrktblog-content-openapi.yml\n  - openapi/advantage-solutions-youradv-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advantage-solutions/refs/heads/main/authentication/advantage-solutions-authentication.yml
summary_line: http · 1 scheme
tags:
- Sales
- Marketing
- Merchandising
- Consumer Goods
- Retail
- Shopper Insights
- Content
- Fortune 500
---
