---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datasette-openapi-generated.yml
  format: yaml
  label: Datasette API
  slug: datasette-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasette/openapi/_ae-authored/datasette-openapi-generated.yml
auth_types: []
description: Authentication schemes documented for Datasette
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Datasette Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datasette declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Datasette
provider_slug: datasette
scheme_count: 2
schemes:
- evidence: The URL on the first line includes a one-use token which can be used to sign in as the "root" actor in your browser.
  location: query
  name: token
  type: apiKey
- evidence: Datasette includes a default authentication plugin which looks for a signed ds_actor cookie containing a JSON actor dictionary.
  header: Cookie
  location: header
  name: ds_actor
  type: other
slug: datasette-authentication
source_filename: datasette-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.datasette.io/en/stable/authentication.html
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.datasette.io/en/stable/authentication.html\nsources:\n- https://docs.datasette.io/en/stable/authentication.html\n- https://docs.datasette.io/en/stable/getting_started.html\ndescription: Authentication schemes documented for Datasette\nschemes:\n- type: apiKey\n  name: token\n  evidence: The URL on the first line includes a one-use token which can be used to sign in as the \"root\" actor in your browser.\n  location: query\n- type: other\n  name: ds_actor\n  evidence: Datasette includes a default authentication plugin which looks for a signed ds_actor cookie containing a JSON actor dictionary.\n  location: header\n  header: Cookie\ndocs: https://docs.datasette.io/en/stable/authentication.html\n"
source_yaml_url: https://artifacts.apis.io/datasette/authentication/datasette-authentication.yml
summary_line: 2 schemes
tags:
- OpenSource
- DataTools
- Publishing
- Visualization
- Community
---
