---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bounceexchange-contacts-api-openapi.yml
  format: yaml
  label: Bounceexchange Contacts API
  slug: bounceexchange-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/bounceexchange-contacts-api-openapi.yml
- filename: bounceexchange-createcontactactivities-api-openapi.yml
  format: yaml
  label: Bounceexchange Createcontactactivities API
  slug: bounceexchange-createcontactactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/bounceexchange-createcontactactivities-api-openapi.yml
- filename: bounceexchange-id-resolution-api-openapi.yml
  format: yaml
  label: Bounceexchange Id Resolution API
  slug: bounceexchange-id-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/bounceexchange-id-resolution-api-openapi.yml
- filename: bounceexchange-interaction-api-openapi.yml
  format: yaml
  label: Bounceexchange Interaction API
  slug: bounceexchange-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/bounceexchange-interaction-api-openapi.yml
- filename: bounceexchange-text-api-openapi.yml
  format: yaml
  label: Bounceexchange Text API
  slug: bounceexchange-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bounceexchange/refs/heads/main/openapi/bounceexchange-text-api-openapi.yml
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
