---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for YubHub API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Yubhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: YubHub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: YubHub
provider_slug: yubhub
scheme_count: 1
schemes:
- evidence: '"bearer_methods_supported": ["header"]'
  header: Authorization
  location: header
  name: OAuth2
  type: oauth2
slug: yubhub-authentication
source_filename: yubhub-authentication.yml
source_heading: Authentication Profile
source_url: https://yubhub.co/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://yubhub.co/.well-known/oauth-protected-resource\nsources:\n- https://yubhub.co/.well-known/oauth-protected-resource\n- https://yubhub.co/developers.md\ndescription: Authentication methods for YubHub API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"bearer_methods_supported\": [\"header\"]'\n  location: header\n  header: Authorization\ndocs: https://yubhub.co/.well-known/oauth-protected-resource\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/yubhub/authentication/yubhub-authentication.yml
summary_line: 1 scheme
tags:
- JobFeed
- Recruitment
- API
- UK
- DataEnrichment
---
