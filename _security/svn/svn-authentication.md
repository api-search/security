---
api_key_in: []
api_specs:
- filename: svn-webdav-openapi.yml
  format: yaml
  label: SVN WebDAV HTTP API
  slug: svn-webdav-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svn/refs/heads/main/openapi/svn-webdav-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Svn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Subversion secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Subversion
provider_slug: svn
scheme_count: 2
schemes:
- description: HTTP Basic authentication for SVN repository access
  name: basicAuth
  scheme: basic
  sources:
  - openapi/svn-webdav-openapi.yml
  type: http
- description: HTTP Digest authentication for SVN repository access
  name: digestAuth
  scheme: digest
  sources:
  - openapi/svn-webdav-openapi.yml
  type: http
slug: svn-authentication
source_filename: svn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/svn-webdav-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication for SVN repository access\n  sources:\n  - openapi/svn-webdav-openapi.yml\n- name: digestAuth\n  type: http\n  scheme: digest\n  description: HTTP Digest authentication for SVN repository access\n  sources:\n  - openapi/svn-webdav-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svn/refs/heads/main/authentication/svn-authentication.yml
summary_line: http · 2 schemes
tags:
- Apache
- Open Source
- Repository
- Source Control
- Svn
- Version Control
- Webdav
---
