---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jackett-openapi-generated.yml
  format: yaml
  label: Jackett API
  slug: jackett-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jackett/openapi/_ae-authored/jackett-openapi-generated.yml
auth_types: []
description: Authentication schemes documented for the provider.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jackett Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jackett declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jackett
provider_slug: jackett
scheme_count: 1
schemes:
- evidence: 'Adding basic auth ¶ By default there is no authentication . On anything other than a trusted LAN, set at minimum: -e CUSTOM_USER = me \ -e PASSWORD = changeme \ This enables HTTP basic auth.'
  header: Authorization
  how_to_obtain: Set environment variables CUSTOM_USER and PASSWORD
  location: header
  name: HTTP Basic Auth
  type: http-basic
slug: jackett-authentication
source_filename: jackett-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.linuxserver.io/images/docker-ldap-auth/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.linuxserver.io/images/docker-ldap-auth/\nsources:\n- https://docs.linuxserver.io/images/docker-ldap-auth/\n- https://docs.linuxserver.io/selkies/user-guide/quickstart/\ndescription: Authentication schemes documented for the provider.\nschemes:\n- type: http-basic\n  name: HTTP Basic Auth\n  evidence: 'Adding basic auth ¶ By default there is no authentication . On anything other than a trusted LAN, set at minimum: -e CUSTOM_USER\n    = me \\ -e PASSWORD = changeme \\ This enables HTTP basic auth.'\n  location: header\n  header: Authorization\n  how_to_obtain: Set environment variables CUSTOM_USER and PASSWORD\ndocs: https://docs.linuxserver.io/images/docker-ldap-auth/\n"
source_yaml_url: https://artifacts.apis.io/jackett/authentication/jackett-authentication.yml
summary_line: 1 scheme
tags:
- Company
- OpenSource
- Torrent
- Proxy
- API
---
