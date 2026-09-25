---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fossil-scm-openapi-generated.yml
  format: yaml
  label: Fossil SCM API
  slug: fossil-scm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/openapi/_ae-authored/fossil-scm-openapi-generated.yml
auth_types: []
description: Authentication methods described in Fossil documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fossil Scm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fossil SCM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fossil SCM
provider_slug: fossil-scm
scheme_count: 2
schemes:
- evidence: If they match, the server sets a cookie on the client to record the login.
  header: Cookie
  how_to_obtain: Obtained after a successful login via the web interface; the server returns a Set-Cookie header.
  location: header
  name: session cookie
  type: apiKey
- evidence: The client normally gets the login and password from the "remote URL". http://login:password@servername.org/path
  header: Authorization
  how_to_obtain: Credentials are supplied as user:password in the repository URL used for sync, push, pull, or clone operations.
  location: header
  name: sync protocol credentials
  type: http-basic
slug: fossil-scm-authentication
source_filename: fossil-scm-authentication.yml
source_heading: Authentication Profile
source_url: https://fossil-scm.org/home/doc/trunk/www/password.wiki
source_yaml: "generated: '2026-09-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fossil-scm.org/home/doc/trunk/www/password.wiki\nsources:\n- https://fossil-scm.org/home/doc/trunk/www/password.wiki\n- https://fossil-scm.org/home/doc/trunk/www/quickstart.wiki\n- https://fossil-scm.org/home/doc/trunk/www/caps/admin-v-setup.md\ndescription: Authentication methods described in Fossil documentation\nschemes:\n- type: apiKey\n  name: session cookie\n  evidence: If they match, the server sets a cookie on the client to record the login.\n  location: header\n  header: Cookie\n  how_to_obtain: Obtained after a successful login via the web interface; the server returns a Set-Cookie header.\n- type: http-basic\n  name: sync protocol credentials\n  evidence: The client normally gets the login and password from the \"remote URL\". http://login:password@servername.org/path\n  location: header\n  header: Authorization\n  how_to_obtain: Credentials are supplied as user:password\
  \ in the repository URL used for sync, push, pull, or clone operations.\ndocs: https://fossil-scm.org/home/doc/trunk/www/password.wiki\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/authentication/fossil-scm-authentication.yml
summary_line: 2 schemes
tags:
- Version Control
- Open Source
- SCM
- Distributed
- Configuration Management
---
