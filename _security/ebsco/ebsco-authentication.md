---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ebsco-content-api-openapi.yml
  format: yaml
  label: EBSCO Content API
  slug: ebsco-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/openapi/ebsco-content-api-openapi.yml
- filename: ebsco-publishers-api-openapi.yml
  format: yaml
  label: EBSCO Publishers API
  slug: ebsco-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/openapi/ebsco-publishers-api-openapi.yml
auth_types: []
description: Authentication methods for EBSCO APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ebsco Authentication
name_suffix: Authentication
oauth_flows: []
overview: EBSCO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EBSCO
provider_slug: ebsco
scheme_count: 2
schemes:
- authorize_url: https://logon.ebsco.zone/api/dispatcher/oauth/authorize
  evidence: EBSCOhost API Beta uses the OAuth 2.0 **authorization code grant** to give each user, or each guest visitor, their own access token.
  flows:
  - authorization_code
  how_to_obtain: Register a client app to receive a Client ID and Client Secret.
  name: EBSCO OAuth
  type: oauth2
- evidence: 'All requests to HoldingsIQ must contain the following API key header field: **x-api-key** {Unique API key as a string}'
  header: x-api-key
  how_to_obtain: Request an API key via the Request API Key Information form.
  location: header
  name: x-api-key
  type: apiKey
slug: ebsco-authentication
source_filename: ebsco-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.ebsco.com/ebscohost-api/docs/authentication-and-access-tokens.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.ebsco.com/ebscohost-api/docs/authentication-and-access-tokens.md\nsources:\n- https://developer.ebsco.com/ebscohost-api/docs/authentication-and-access-tokens.md\n- https://developer.ebsco.com/ebscohost-api/docs/authentication-concepts.md\n- https://developer.ebsco.com/home/page/request-api-key-information.md\n- https://developer.ebsco.com/knowledge-services/docs/holdingsiq-authentication.md\ndescription: Authentication methods for EBSCO APIs\nschemes:\n- type: oauth2\n  name: EBSCO OAuth\n  evidence: EBSCOhost API Beta uses the OAuth 2.0 **authorization code grant** to give each user, or each guest visitor, their own access token.\n  flows:\n  - authorization_code\n  authorize_url: https://logon.ebsco.zone/api/dispatcher/oauth/authorize\n  how_to_obtain: Register a client app to receive a Client ID and Client Secret.\n- type: apiKey\n  name: x-api-key\n  evidence:\
  \ 'All requests to HoldingsIQ must contain the following API key header field: **x-api-key** {Unique API key as a string}'\n  location: header\n  header: x-api-key\n  how_to_obtain: Request an API key via the Request API Key Information form.\ndocs: https://developer.ebsco.com/ebscohost-api/docs/authentication-and-access-tokens.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/authentication/ebsco-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Research
- Library
- Education
- Information
---
