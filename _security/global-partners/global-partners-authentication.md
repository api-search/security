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
name: Global Partners Authentication
name_suffix: Authentication
oauth_flows: []
overview: Global Partners LP secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Global Partners LP
provider_slug: global-partners
scheme_count: 1
schemes:
- description: WordPress application passwords (HTTP Basic). The site's discovery document advertises the authorization endpoint at https://www.globalp.com/wp-admin/authorize-application.php. Read operations require no credentials.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/global-partners-categories-api-openapi.yml
  - openapi/global-partners-comments-api-openapi.yml
  - openapi/global-partners-content-media-type-api-openapi.yml
  - openapi/global-partners-content-topic-api-openapi.yml
  - openapi/global-partners-content-type-api-openapi.yml
  - openapi/global-partners-media-api-openapi.yml
  - openapi/global-partners-pages-api-openapi.yml
  - openapi/global-partners-posts-api-openapi.yml
  - openapi/global-partners-search-api-openapi.yml
  - openapi/global-partners-statuses-api-openapi.yml
  - openapi/global-partners-sw-business-sector-api-openapi.yml
  - openapi/global-partners-sw-employee-api-openapi.yml
  - openapi/global-partners-sw-food-option-api-openapi.yml
  - openapi/global-partners-sw-fuel-brand-api-openapi.yml
  - openapi/global-partners-sw-fuel-type-api-openapi.yml
  - openapi/global-partners-sw-listing-type-api-openapi.yml
  - openapi/global-partners-sw-method-of-supply-api-openapi.yml
  - openapi/global-partners-sw-ownership-status-api-openapi.yml
  - openapi/global-partners-sw-product-api-openapi.yml
  - openapi/global-partners-sw-property-api-openapi.yml
  - openapi/global-partners-sw-retail-brand-api-openapi.yml
  - openapi/global-partners-sw-retail-location-api-openapi.yml
  - openapi/global-partners-sw-service-api-openapi.yml
  - openapi/global-partners-sw-site-type-api-openapi.yml
  - openapi/global-partners-sw-state-api-openapi.yml
  - openapi/global-partners-sw-terminal-api-openapi.yml
  - openapi/global-partners-tags-api-openapi.yml
  - openapi/global-partners-taxonomies-api-openapi.yml
  - openapi/global-partners-types-api-openapi.yml
  - openapi/global-partners-users-api-openapi.yml
  type: http
slug: global-partners-authentication
source_filename: global-partners-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/global-partners-categories-api-openapi.yml, openapi/global-partners-comments-api-openapi.yml,\n  openapi/global-partners-content-media-type-api-openapi.yml, openapi/global-partners-content-topic-api-openapi.yml,\n  openapi/global-partners-content-type-api-openapi.yml, openapi/global-partners-media-api-openapi.yml,\n  openapi/global-partners-pages-api-openapi.yml, openapi/global-partners-posts-api-openapi.yml,\n  openapi/global-partners-search-api-openapi.yml, openapi/global-partners-statuses-api-openapi.yml,\n  openapi/global-partners-sw-business-sector-api-openapi.yml, openapi/global-partners-sw-employee-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords (HTTP Basic). The site's discovery document advertises\n    the authorization endpoint at https://www.globalp.com/wp-admin/authorize-application.php.\n\
  \    Read operations require no credentials.\n  sources:\n  - openapi/global-partners-categories-api-openapi.yml\n  - openapi/global-partners-comments-api-openapi.yml\n  - openapi/global-partners-content-media-type-api-openapi.yml\n  - openapi/global-partners-content-topic-api-openapi.yml\n  - openapi/global-partners-content-type-api-openapi.yml\n  - openapi/global-partners-media-api-openapi.yml\n  - openapi/global-partners-pages-api-openapi.yml\n  - openapi/global-partners-posts-api-openapi.yml\n  - openapi/global-partners-search-api-openapi.yml\n  - openapi/global-partners-statuses-api-openapi.yml\n  - openapi/global-partners-sw-business-sector-api-openapi.yml\n  - openapi/global-partners-sw-employee-api-openapi.yml\n  - openapi/global-partners-sw-food-option-api-openapi.yml\n  - openapi/global-partners-sw-fuel-brand-api-openapi.yml\n  - openapi/global-partners-sw-fuel-type-api-openapi.yml\n  - openapi/global-partners-sw-listing-type-api-openapi.yml\n  - openapi/global-partners-sw-method-of-supply-api-openapi.yml\n\
  \  - openapi/global-partners-sw-ownership-status-api-openapi.yml\n  - openapi/global-partners-sw-product-api-openapi.yml\n  - openapi/global-partners-sw-property-api-openapi.yml\n  - openapi/global-partners-sw-retail-brand-api-openapi.yml\n  - openapi/global-partners-sw-retail-location-api-openapi.yml\n  - openapi/global-partners-sw-service-api-openapi.yml\n  - openapi/global-partners-sw-site-type-api-openapi.yml\n  - openapi/global-partners-sw-state-api-openapi.yml\n  - openapi/global-partners-sw-terminal-api-openapi.yml\n  - openapi/global-partners-tags-api-openapi.yml\n  - openapi/global-partners-taxonomies-api-openapi.yml\n  - openapi/global-partners-types-api-openapi.yml\n  - openapi/global-partners-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-partners/refs/heads/main/authentication/global-partners-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Fuel Distribution
- Oil and Gas
- Petroleum
- Retail Fuel
- Terminal
- Fortune 500
- Content
- WordPress
- Terminal Network
- Retail Locations
---
