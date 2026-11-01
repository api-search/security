---
anonymous_access: false
api_key_in: []
auth_types: []
description: Machine-to-Machine (M2M) authentication based on OAuth 2.0 with client_credentials grant type.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Immowelt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immowelt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Immowelt
provider_slug: immowelt
scheme_count: 1
schemes:
- evidence: This API uses **Machine-to-Machine (M2M) authentication** based on OAuth 2.0 with `client_credentials` grant type.
  flows:
  - client_credentials
  how_to_obtain: client_id and client_secret are provided by Immowelt (and an optional intermediary_id for some APIs).
  name: OAuth 2.0 Client Credentials
  token_url: https://auth.apim.immowelt.de/oauth/token
  type: oauth2
slug: immowelt-authentication
source_filename: immowelt-authentication.yml
source_heading: Authentication Profile
source_url: https://227098cb35ba.eu.kongportals.com/apis/seeker-leads-de-v1/docs/m2m-authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://227098cb35ba.eu.kongportals.com/apis/seeker-leads-de-v1/docs/m2m-authentication.md\nsources:\n- https://227098cb35ba.eu.kongportals.com/apis/seeker-leads-de-v1/docs/m2m-authentication.md\n- https://227098cb35ba.eu.kongportals.com/apis/export-listings-v1/docs/m2m-authentication.md\n- https://227098cb35ba.eu.kongportals.com/apis/import-listings-v1/docs/m2m-authentication.md\n- https://227098cb35ba.eu.kongportals.com/apis/seeker-leads-ingest-de-v1/docs/m2m-authentication.md\ndescription: Machine-to-Machine (M2M) authentication based on OAuth 2.0 with client_credentials grant type.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Client Credentials\n  evidence: This API uses **Machine-to-Machine (M2M) authentication** based on OAuth 2.0 with `client_credentials` grant type.\n  flows:\n  - client_credentials\n  token_url: https://auth.apim.immowelt.de/oauth/token\n  how_to_obtain:\
  \ client_id and client_secret are provided by Immowelt (and an optional intermediary_id for some APIs).\ndocs: https://227098cb35ba.eu.kongportals.com/apis/seeker-leads-de-v1/docs/m2m-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/immowelt/authentication/immowelt-authentication.yml
summary_line: 1 scheme
tags:
- Real Estate
- Marketplace
- Germany
- Austria
- Property Listings
---
