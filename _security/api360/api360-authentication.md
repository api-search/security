---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on the API360 documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: API360 Authentication
name_suffix: Authentication
oauth_flows: []
overview: API360 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: API360
provider_slug: api360
scheme_count: 2
schemes:
- evidence: 'Every request to a product carries a credential of the app that makes it: an API key in the api360key header, or an HTTP Basic username and password.'
  header: api360key
  how_to_obtain: Created on the Authorization tab of an app; the platform generates a 64‑character random string and shows it in the app’s Authorization tab.
  location: header
  name: api360key
  type: apiKey
- evidence: Authorization Basic and the base64 of username:password only with a credential of type Basic auth
  header: Authorization
  how_to_obtain: Created on the Authorization tab of an app; the platform generates a UUID username and a 64‑character password and shows them in the app’s Authorization tab.
  location: header
  name: basic
  type: http-basic
slug: api360-authentication
source_filename: api360-authentication.yml
source_heading: Authentication Profile
source_url: https://api360.sa/docs/reference/authentication?lang=en
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api360.sa/docs/reference/authentication?lang=en\nsources:\n- https://api360.sa/docs/reference/authentication?lang=en\n- https://api360.sa/docs/reference/authentication\n- https://api360.sa/docs?lang=en\n- https://api360.sa/_sitepages/docs-img/ar/consumer/apps-and-keys/add-auth.png\ndescription: Authentication methods as published on the API360 documentation pages.\nschemes:\n- type: apiKey\n  name: api360key\n  evidence: 'Every request to a product carries a credential of the app that makes it: an API key in the api360key header, or an HTTP Basic username\n    and password.'\n  location: header\n  header: api360key\n  how_to_obtain: Created on the Authorization tab of an app; the platform generates a 64‑character random string and shows it in the app’s Authorization\n    tab.\n- type: http-basic\n  name: basic\n  evidence: Authorization Basic and the base64 of username:password\
  \ only with a credential of type Basic auth\n  location: header\n  header: Authorization\n  how_to_obtain: Created on the Authorization tab of an app; the platform generates a UUID username and a 64‑character password and shows them\n    in the app’s Authorization tab.\ndocs: https://api360.sa/docs/reference/authentication?lang=en\n"
source_yaml_url: https://artifacts.apis.io/api360/authentication/api360-authentication.yml
summary_line: 2 schemes
tags:
- Saudi Arabia
- API Marketplace
- Government APIs
- Open Banking
- Integration
---
