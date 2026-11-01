---
anonymous_access: false
api_key_in: []
api_specs:
- filename: like-magic-openapi-generated.yml
  format: yaml
  label: LIKE MAGIC API
  slug: like-magic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/like-magic/openapi/_ae-authored/like-magic-openapi-generated.yml
auth_types: []
description: Authentication for LikeMagic public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Like Magic Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIKE MAGIC declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LIKE MAGIC
provider_slug: like-magic
scheme_count: 1
schemes:
- evidence: We use OAuth 2.0 Client Credentials Flow - the standard for server-to-server authentication.
  flows:
  - client_credentials
  how_to_obtain: Client credentials (clientId and clientSecret) are obtained by creating a service account in the Operations Platform by an Account Admin.
  name: OAuth 2.0 Client Credentials
  scopes:
  - guest_conversation.write
  - event_log.read
  token_url: '{{tokenEndpoint}}'
  type: oauth2
slug: like-magic-authentication
source_filename: like-magic-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.likemagic.tech/docs/developer-api/public-api-and-authentication/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.likemagic.tech/docs/developer-api/public-api-and-authentication/\nsources:\n- https://docs.likemagic.tech/docs/developer-api/public-api-and-authentication/\n- https://api-docs.likemagic.tech/guide/setup/authentication/\n- https://docs.likemagic.tech/docs/category/getting-started/\n- https://docs.likemagic.tech/docs/getting-started/configure-property-settings/\ndescription: Authentication for LikeMagic public API\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Client Credentials\n  evidence: We use OAuth 2.0 Client Credentials Flow - the standard for server-to-server authentication.\n  flows:\n  - client_credentials\n  token_url: '{{tokenEndpoint}}'\n  scopes:\n  - guest_conversation.write\n  - event_log.read\n  how_to_obtain: Client credentials (clientId and clientSecret) are obtained by creating a service account in the Operations Platform by an Account\n    Admin.\n\
  docs: https://docs.likemagic.tech/docs/developer-api/public-api-and-authentication/\n"
source_yaml_url: https://artifacts.apis.io/like-magic/authentication/like-magic-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hospitality
- Technology
- Guest Experience
- Hotel Operations
---
