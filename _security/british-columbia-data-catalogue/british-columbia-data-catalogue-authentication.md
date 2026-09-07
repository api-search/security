---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: british-columbia-data-catalogue-bcdc-api-openapi.json
  format: json
  label: BC Data Catalogue CKAN API
  slug: ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-bcdc-api-openapi.json
- filename: british-columbia-data-catalogue-datasets-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Datasets API
  slug: british-columbia-data-catalogue-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-datasets-api-openapi.yml
- filename: british-columbia-data-catalogue-groups-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Groups API
  slug: british-columbia-data-catalogue-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-groups-api-openapi.yml
- filename: british-columbia-data-catalogue-organizations-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Organizations API
  slug: british-columbia-data-catalogue-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-organizations-api-openapi.yml
- filename: british-columbia-data-catalogue-resources-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Resources API
  slug: british-columbia-data-catalogue-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-resources-api-openapi.yml
- filename: british-columbia-data-catalogue-site-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Site API
  slug: british-columbia-data-catalogue-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-site-api-openapi.yml
- filename: british-columbia-data-catalogue-tags-api-openapi.yml
  format: yaml
  label: British Columbia Data Catalogue Tags API
  slug: british-columbia-data-catalogue-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-tags-api-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: British Columbia Data Catalogue Authentication
name_suffix: Authentication
oauth_flows: []
overview: British Columbia Data Catalogue secures its APIs with none and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: British Columbia Data Catalogue
provider_slug: british-columbia-data-catalogue
scheme_count: 3
schemes:
- applies_to: all public read actions
  detail: package_search, package_list, package_show, organization_*, group_*, tag_* and resource_* answered anonymously on every probe.
  evidence: https://catalogue.data.gov.bc.ca/api/3/action/status_show
  name: none
  type: none
- applies_to: write actions
  evidence:
    body: '{"error": {"__type": "Authorization Error", "message": "Access denied: User  not authorized to create packages"}, "success": false}'
    method: POST
    status: 403
    url: https://catalogue.data.gov.bc.ca/api/3/action/package_create
  in: header
  name: internalApiKey
  obtained_from: Account Settings after signing in to catalogue.data.gov.bc.ca. Requires editor/publisher rights in a B.C. government organization — an internal entitlement, not a self-service signup.
  parameter: ckan_api_key
  sources:
  - openapi/british-columbia-data-catalogue-bcdc-api-openapi.json
  - https://bcgov.github.io/data-publication/pages/dps_bcdc_api_w_resource_mgmt.html
  type: apiKey
- applies_to: nothing
  declared_in: openapi/british-columbia-data-catalogue-bcdc-api-openapi.json
  disregard: true
  finding: This oauth2 scheme is Swagger-editor boilerplate, NOT a BC Data Catalogue authorization server. Its endpoints are github.com and its 19 scopes are GitHub's own (repo, gist, delete_repo, admin:org, write:public_key). Treating it as a BC OAuth surface would credit the Province with an authorization server it does not operate and would hand an agent a scope list that has nothing to do with B.C. data. No OAuthScopes artifact or pointer is emitted for this provider for the same reason.
  flows:
  - authorizationUrl: https://github.com/login/oauth/authorize
    flow: authorizationCode
    scopes: 19
    tokenUrl: https://github.com/login/oauth/access_token
  name: githubAccessCode
  remedy: Removing the githubAccessCode block from bcdc.json, or replacing it with the catalogue's real OpenID Connect metadata, would make the contract's security section truthful.
  type: oauth2
slug: british-columbia-data-catalogue-authentication
source_filename: british-columbia-data-catalogue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/british-columbia-data-catalogue-bcdc-api-openapi.json (the first-party spec),\n  https://bcgov.github.io/data-publication/pages/dps_bcdc_api_w_how_to_use.html,\n  https://bcgov.github.io/data-publication/pages/dps_bcdc_api_w_resource_mgmt.html, and a\n  live probe of POST /api/3/action/package_create.\ndocs: https://bcgov.github.io/data-publication/pages/dps_bcdc_api_w_how_to_use.html\nprovider: British Columbia Data Catalogue\nproviderId: british-columbia-data-catalogue\nsummary:\n  types:\n    - none\n    - apiKey\n  api_key_in:\n    - header\n  read_access: anonymous\n  write_access: api-key\nheadline: >-\n  Public reads need no credential at all. DataBC states it plainly: \"You do not need an API\n  key nor an account if you are only accessing publicly available data.\" Writes need a\n  catalogue account with editor/publisher rights and its token in the ckan_api_key header.\nschemes:\n  - name: none\n    type:\
  \ none\n    applies_to: all public read actions\n    detail: >-\n      package_search, package_list, package_show, organization_*, group_*, tag_* and\n      resource_* answered anonymously on every probe.\n    evidence: https://catalogue.data.gov.bc.ca/api/3/action/status_show\n  - name: internalApiKey\n    type: apiKey\n    in: header\n    parameter: ckan_api_key\n    applies_to: write actions\n    obtained_from: >-\n      Account Settings after signing in to catalogue.data.gov.bc.ca. Requires\n      editor/publisher rights in a B.C. government organization — an internal entitlement,\n      not a self-service signup.\n    sources:\n      - openapi/british-columbia-data-catalogue-bcdc-api-openapi.json\n      - https://bcgov.github.io/data-publication/pages/dps_bcdc_api_w_resource_mgmt.html\n    evidence:\n      url: https://catalogue.data.gov.bc.ca/api/3/action/package_create\n      method: POST\n      status: 403\n      body: '{\"error\": {\"__type\": \"Authorization Error\", \"message\"\
  : \"Access denied: User  not authorized to create packages\"}, \"success\": false}'\n  - name: githubAccessCode\n    type: oauth2\n    applies_to: nothing\n    disregard: true\n    declared_in: openapi/british-columbia-data-catalogue-bcdc-api-openapi.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://github.com/login/oauth/authorize\n        tokenUrl: https://github.com/login/oauth/access_token\n        scopes: 19\n    finding: >-\n      This oauth2 scheme is Swagger-editor boilerplate, NOT a BC Data Catalogue\n      authorization server. Its endpoints are github.com and its 19 scopes are GitHub's own\n      (repo, gist, delete_repo, admin:org, write:public_key). Treating it as a BC OAuth\n      surface would credit the Province with an authorization server it does not operate\n      and would hand an agent a scope list that has nothing to do with B.C. data. No\n      OAuthScopes artifact or pointer is emitted for this provider for the same reason.\n \
  \   remedy: >-\n      Removing the githubAccessCode block from bcdc.json, or replacing it with the\n      catalogue's real OpenID Connect metadata, would make the contract's security section\n      truthful.\nsso:\n  protocol: OpenID Connect\n  applies_to: interactive sign-in to the catalogue web application\n  evidence:\n    - url: https://catalogue.data.gov.bc.ca/api/3/action/status_show\n      note: 'extensions[] includes \"sso\"'\n    - url: https://github.com/bcgov/ckanext-sso\n      note: '\"OpenID connect plugin for CKAN used by the B.C. Catalogue.\"'\n  discovery_document: null\n  discovery_note: >-\n    No /.well-known/openid-configuration is served on any host in this record — every\n    probe returned the SPA catch-all or a 404. See\n    well-known/british-columbia-data-catalogue-well-known.yml.\nmtls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/authentication/british-columbia-data-catalogue-authentication.yml
summary_line: none/apiKey · 3 schemes
tags:
- Open Data
- Government
- Canadian Government
- British Columbia
- Provincial Data
- CKAN
- Geospatial
- OGC
- WMS
- WFS
- Dataset Search
- Public Sector
---
