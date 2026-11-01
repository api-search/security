---
anonymous_access: false
api_key_in: []
auth_types: []
description: Basic authentication is handled by Nginx using HTTP Basic auth.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Unmanic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unmanic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Unmanic
provider_slug: unmanic
scheme_count: 1
schemes:
- evidence: Unmanic can use basic authentication when connecting to another instance.
  header: Authorization
  location: header
  name: Basic
  type: http-basic
slug: unmanic-authentication
source_filename: unmanic-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.unmanic.app/docs/guides/basic_auth_nginx/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.unmanic.app/docs/guides/basic_auth_nginx/\nsources:\n- https://docs.unmanic.app/docs/guides/basic_auth_nginx/\n- https://docs.unmanic.app/docs/using_unmanic/getting_started/\n- https://docs.unmanic.app/docs/\ndescription: Basic authentication is handled by Nginx using HTTP Basic auth.\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: Unmanic can use basic authentication when connecting to another instance.\n  location: header\n  header: Authorization\ndocs: https://docs.unmanic.app/docs/guides/basic_auth_nginx/\n"
source_yaml_url: https://artifacts.apis.io/unmanic/authentication/unmanic-authentication.yml
summary_line: 1 scheme
tags:
- Media
- Automation
- OpenSource
- FileManagement
- Optimization
---
