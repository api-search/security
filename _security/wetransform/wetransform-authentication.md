---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wetransform-openapi-generated.yml
  format: yaml
  label: WeTransform API
  slug: wetransform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wetransform/openapi/_ae-authored/wetransform-openapi-generated.yml
auth_types: []
description: Authentication is performed using HMAC SHA256 signatures included as query parameters in a signed URL.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wetransform Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeTransform declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: WeTransform
provider_slug: wetransform
scheme_count: 1
schemes:
- evidence: This is handled through **HMAC SHA256 signatures** — a secure, invisible handshake between your server and WeTransform.
  location: query
  type: hmac
slug: wetransform-authentication
source_filename: wetransform-authentication.yml
source_heading: Authentication Profile
source_url: https://help.wetransform.com/en/articles/14324740-authentication-how-to-make-the-experience-seamless-for-your-clients.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.wetransform.com/en/articles/14324740-authentication-how-to-make-the-experience-seamless-for-your-clients.md\nsources:\n- https://help.wetransform.com/en/articles/14324740-authentication-how-to-make-the-experience-seamless-for-your-clients.md\n- https://help.wetransform.com/en/articles/14325197-use-case-remove-the-data-format-barrier-from-client-onboarding.md\ndescription: Authentication is performed using HMAC SHA256 signatures included as query parameters in a signed URL.\nschemes:\n- type: hmac\n  evidence: This is handled through **HMAC SHA256 signatures** — a secure, invisible handshake between your server and WeTransform.\n  location: query\ndocs: https://help.wetransform.com/en/articles/14324740-authentication-how-to-make-the-experience-seamless-for-your-clients.md\n"
source_yaml_url: https://artifacts.apis.io/wetransform/authentication/wetransform-authentication.yml
summary_line: 1 scheme
tags:
- Data Integration
- B2B SaaS
- No-Code
- Artificial Intelligence
- Embedded Import
---
