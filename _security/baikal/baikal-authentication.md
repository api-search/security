---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods supported by Baïkal (sabre/dav) as described on the documentation page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Baikal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baikal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Baikal
provider_slug: baikal
scheme_count: 2
schemes:
- evidence: The standard way to do this, is to add HTTP Basic or HTTP Digest authentication support.
  header: Authorization
  how_to_obtain: Provide a username and password (e.g., via the Authorization header using the Basic scheme).
  location: header
  name: HTTP Basic
  type: http-basic
- evidence: The standard way to do this, is to add HTTP Basic or HTTP Digest authentication support.
  header: Authorization
  how_to_obtain: Provide a username, password, and realm; the server expects a Digest response in the Authorization header.
  location: header
  name: HTTP Digest
  type: other
slug: baikal-authentication
source_filename: baikal-authentication.yml
source_heading: Authentication Profile
source_url: https://sabre.io/dav/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sabre.io/dav/authentication/\nsources:\n- https://sabre.io/dav/authentication/\ndescription: Authentication methods supported by Baïkal (sabre/dav) as described on the documentation page.\nschemes:\n- type: http-basic\n  name: HTTP Basic\n  evidence: The standard way to do this, is to add HTTP Basic or HTTP Digest authentication support.\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a username and password (e.g., via the Authorization header using the Basic scheme).\n- type: other\n  name: HTTP Digest\n  evidence: The standard way to do this, is to add HTTP Basic or HTTP Digest authentication support.\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a username, password, and realm; the server expects a Digest response in the Authorization header.\ndocs: https://sabre.io/dav/authentication/\n"
source_yaml_url: https://artifacts.apis.io/baikal/authentication/baikal-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- OpenSource
- Calendar
- CardDAV
---
