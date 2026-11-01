---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes published for Fiorano ESB 13.2
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fiorano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiorano Software declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fiorano Software
provider_slug: fiorano
scheme_count: 1
schemes:
- evidence: When Fiorano RestStub checks for the query parameter "APIKey", if it is not found, it checks for the Header Param "APIKey" and validates the user if the user has the permission to invoke that particular service.
  header: APIKey
  how_to_obtain: Created in the Dashboard under Security tab for REST services; the generated API Key is copied and used in requests.
  location: query/header
  name: APIKey
  type: apiKey
slug: fiorano-authentication
source_filename: fiorano-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fiorano.com/esb/13.2/authentication.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fiorano.com/esb/13.2/authentication.md\nsources:\n- https://docs.fiorano.com/esb/13.2/authentication.md\n- https://docs.fiorano.com/esb/13.2/authentication-and-authorization.md\n- https://docs.fiorano.com/esb/13.2/extending-authentication.md\n- https://docs.fiorano.com/esb/13.2/using-api-key-in-the-reststub-microservice.md\ndescription: Authentication schemes published for Fiorano ESB 13.2\nschemes:\n- type: apiKey\n  name: APIKey\n  evidence: When Fiorano RestStub checks for the query parameter \"APIKey\", if it is not found, it checks for the Header Param \"APIKey\" and validates\n    the user if the user has the permission to invoke that particular service.\n  location: query/header\n  header: APIKey\n  how_to_obtain: Created in the Dashboard under Security tab for REST services; the generated API Key is copied and used in requests.\ndocs: https://docs.fiorano.com/esb/13.2/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/fiorano/authentication/fiorano-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Integration
- API Management
- Enterprise
- Messaging
---
