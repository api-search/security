---
anonymous_access: false
api_key_in: []
api_specs:
- filename: directree-io-listings-api-openapi.yml
  format: yaml
  label: Directree Listings API
  slug: directree-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/directree-io/openapi/directree-io-listings-api-openapi.yml
auth_types: []
description: Directree API uses a simple bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Directree Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Directree declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Directree
provider_slug: directree-io
scheme_count: 1
schemes:
- evidence: 'Authentication is Authorization: Bearer YOUR_API_KEY.'
  header: Authorization
  how_to_obtain: Create a connection in the Directree dashboard and copy the generated key, then store it as DIRECTREE_API_KEY.
  location: header
  name: Bearer API Key
  type: http-bearer
slug: directree-io-authentication
source_filename: directree-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.directree.io/category/security-auth
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.directree.io/category/security-auth\nsources:\n- https://www.directree.io/category/security-auth\n- https://www.directree.io/docs/agent-api\ndescription: Directree API uses a simple bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer API Key\n  evidence: 'Authentication is Authorization: Bearer YOUR_API_KEY.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a connection in the Directree dashboard and copy the generated key, then store it as DIRECTREE_API_KEY.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://www.directree.io/category/security-auth\n"
source_yaml_url: https://artifacts.apis.io/directree-io/authentication/directree-io-authentication.yml
summary_line: 1 scheme
tags:
- Software-as-a-Service
- Directory
- Software
- Reviews
- Open Data
---
