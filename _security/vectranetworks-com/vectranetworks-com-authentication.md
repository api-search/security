---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vectranetworks-com-openapi-generated.yml
  format: yaml
  label: Vectranetworks API
  slug: vectranetworks-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vectranetworks-com/openapi/_ae-authored/vectranetworks-com-openapi-generated.yml
auth_types: []
description: Authentication for Vectra QUX APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vectranetworks Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vectranetworks declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vectranetworks
provider_slug: vectranetworks-com
scheme_count: 1
schemes:
- evidence: 'Headers : "Authorization": "Token <api-key>"'
  header: Authorization
  location: header
  name: Token
  type: apiKey
slug: vectranetworks-com-authentication
source_filename: vectranetworks-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.vectra.ai/configuration/access/external-authentication-qux.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.vectra.ai/configuration/access/external-authentication-qux.md\nsources:\n- https://docs.vectra.ai/configuration/access/external-authentication-qux.md\n- https://docs.vectra.ai/configuration/access/external-authentication-qux/radius-qux.md\n- https://docs.vectra.ai/configuration/access/external-authentication-qux/ldap-qux.md\n- https://docs.vectra.ai/configuration/access/external-authentication-qux/tacacs-qux.md\ndescription: Authentication for Vectra QUX APIs\nschemes:\n- type: apiKey\n  name: Token\n  evidence: 'Headers : \"Authorization\": \"Token <api-key>\"'\n  location: header\n  header: Authorization\ndocs: https://docs.vectra.ai/configuration/access/external-authentication-qux.md\n"
source_yaml_url: https://artifacts.apis.io/vectranetworks-com/authentication/vectranetworks-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- AI
- Network
- Threat-Detection
---
