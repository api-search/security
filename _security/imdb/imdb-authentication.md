---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for IMDb API as described on the page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Imdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: IMDb declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: IMDb
provider_slug: imdb
scheme_count: 2
schemes:
- evidence: 'Whenever you make a call to the API you must include the API Key. The API must be passed in as a request header with the following format { "x-api-key": "<Your API Key>" } .'
  header: x-api-key
  how_to_obtain: The API key was sent to you by a member of IMDb staff.
  location: header
  name: API Key
  type: apiKey
- evidence: When you make requests to the IMDb API, you will have to authenticate with AWS by providing some form of AWS credentials.
  how_to_obtain: Obtain AWS credentials as described in the "understanding and getting your AWS credentials" documentation.
  name: AWS Authentication
  type: other
slug: imdb-authentication
source_filename: imdb-authentication.yml
source_heading: Authentication Profile
source_url: https://data.imdb.com/documentation/api-documentation/key-concepts
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://data.imdb.com/documentation/api-documentation/key-concepts\nsources:\n- https://data.imdb.com/documentation/api-documentation/key-concepts\ndescription: Authentication methods for IMDb API as described on the page.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Whenever you make a call to the API you must include the API Key. The API must be passed in as a request header with the following\n    format { \"x-api-key\": \"<Your API Key>\" } .'\n  location: header\n  header: x-api-key\n  how_to_obtain: The API key was sent to you by a member of IMDb staff.\n- type: other\n  name: AWS Authentication\n  evidence: When you make requests to the IMDb API, you will have to authenticate with AWS by providing some form of AWS credentials.\n  how_to_obtain: Obtain AWS credentials as described in the \"understanding and getting your AWS credentials\" documentation.\ndocs: https://data.imdb.com/documentation/api-documentation/key-concepts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imdb/refs/heads/main/authentication/imdb-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Entertainment
- Data
- Movies
- Metadata
---
