---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bounceexchange-openapi-generated.yml
  format: yaml
  label: Bounceexchange API
  slug: bounceexchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/_ae-authored/bounceexchange-openapi-generated.yml
auth_types: []
description: Authentication methods published for Wunderkind (Bounceexchange) APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bounceexchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bounceexchange declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bounceexchange
provider_slug: bounceexchange
scheme_count: 1
schemes:
- evidence: A username and password to be sent via Basic authentication
  header: Authorization
  how_to_obtain: Provided during webhook setup
  location: header
  name: Basic
  type: http-basic
slug: bounceexchange-authentication
source_filename: bounceexchange-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.wunderkind.co/reference/authentication-security.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.wunderkind.co/reference/authentication-security.md\nsources:\n- https://developer.wunderkind.co/reference/authentication-security.md\n- https://developer.wunderkind.co/reference/service_apppushtokenset.md\n- https://developer.wunderkind.co/docs/msdk-getting-started.md\n- https://developer.wunderkind.co/docs/android-apppush-setup-guide.md\ndescription: Authentication methods published for Wunderkind (Bounceexchange) APIs\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: A username and password to be sent via Basic authentication\n  location: header\n  header: Authorization\n  how_to_obtain: Provided during webhook setup\nnote: No other authentication schemes (apiKey, oauth2, http-bearer, jwt, hmac, mtls, other) are documented on the provided pages.\ndocs: https://developer.wunderkind.co/reference/authentication-security.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/authentication/bounceexchange-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
