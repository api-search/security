---
anonymous_access: false
api_key_in: []
auth_types: []
description: YOURLS authenticates users with a username and password defined in the config file. Users log in using their credentials, which are sent via HTTP Basic Authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Yourls Authentication
name_suffix: Authentication
oauth_flows: []
overview: YOURLS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: YOURLS
provider_slug: yourls
scheme_count: 1
schemes:
- evidence: User will still log in using joe as a username and MyPassword as a password, but this password is no longer written down anywhere in the config file.
  header: Authorization
  how_to_obtain: Add a username and password pair to the $yourls_user_passwords array in config.php.
  location: header
  name: Basic Auth
  type: http-basic
slug: yourls-authentication
source_filename: yourls-authentication.yml
source_heading: Authentication Profile
source_url: https://yourls.org/docs/guide/essentials/credentials
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://yourls.org/docs/guide/essentials/credentials\nsources:\n- https://yourls.org/docs/guide/essentials/credentials\n- https://yourls.org/docs/category/getting-started\ndescription: YOURLS authenticates users with a username and password defined in the config file. Users log in using their credentials, which are\n  sent via HTTP Basic Authentication.\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: User will still log in using joe as a username and MyPassword as a password, but this password is no longer written down anywhere\n    in the config file.\n  location: header\n  header: Authorization\n  how_to_obtain: Add a username and password pair to the $yourls_user_passwords array in config.php.\ndocs: https://yourls.org/docs/guide/essentials/credentials\n"
source_yaml_url: https://artifacts.apis.io/yourls/authentication/yourls-authentication.yml
summary_line: 1 scheme
tags:
- Company
- URL-Shortener
- Open-Source
- PHP
- Self-Hosted
---
