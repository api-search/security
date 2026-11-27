---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on the ListingGood developers page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ListingGood Authentication
name_suffix: Authentication
oauth_flows: []
overview: ListingGood declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ListingGood
provider_slug: listinggood-com
scheme_count: 2
schemes:
- evidence: Send your API key as a Bearer token in the request header, or as the apikey query parameter.
  header: Authorization
  how_to_obtain: Log in to ListingGood and copy the API key from the Get API Key section.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Send your API key as a Bearer token in the request header, or as the apikey query parameter.
  how_to_obtain: Log in to ListingGood and copy the API key from the Get API Key section.
  location: query
  name: apikey
  type: apiKey
slug: listinggood-com-authentication
source_filename: listinggood-com-authentication.yml
source_heading: Authentication Profile
source_url: https://listinggood.com/developers
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://listinggood.com/developers\nsources:\n- https://listinggood.com/developers\ndescription: Authentication methods as published on the ListingGood developers page.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Send your API key as a Bearer token in the request header, or as the apikey query parameter.\n  location: header\n  header: Authorization\n  how_to_obtain: Log in to ListingGood and copy the API key from the Get API Key section.\n- type: apiKey\n  name: apikey\n  evidence: Send your API key as a Bearer token in the request header, or as the apikey query parameter.\n  location: query\n  how_to_obtain: Log in to ListingGood and copy the API key from the Get API Key section.\ndocs: https://listinggood.com/developers\n"
source_yaml_url: https://artifacts.apis.io/listinggood-com/authentication/listinggood-com-authentication.yml
summary_line: 2 schemes
tags:
- E-Commerce
- Artificial Intelligence
- Amazon
- Listings
- Compliance
---
