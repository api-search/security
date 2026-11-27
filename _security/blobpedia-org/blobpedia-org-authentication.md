---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blobpedia-org-analytics-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Analytics API
  slug: blobpedia-org-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-analytics-api-openapi.yml
- filename: blobpedia-org-cips-api-openapi.yml
  format: yaml
  label: BLOBPEDIA CIPs API
  slug: blobpedia-org-cips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-cips-api-openapi.yml
- filename: blobpedia-org-discovery-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Discovery API
  slug: blobpedia-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-discovery-api-openapi.yml
- filename: blobpedia-org-discussions-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Discussions API
  slug: blobpedia-org-discussions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-discussions-api-openapi.yml
- filename: blobpedia-org-documentation-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Documentation API
  slug: blobpedia-org-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-documentation-api-openapi.yml
- filename: blobpedia-org-github-api-openapi.yml
  format: yaml
  label: BLOBPEDIA GitHub API
  slug: blobpedia-org-github-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-github-api-openapi.yml
- filename: blobpedia-org-meta-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Meta API
  slug: blobpedia-org-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-meta-api-openapi.yml
- filename: blobpedia-org-network-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Network API
  slug: blobpedia-org-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-network-api-openapi.yml
- filename: blobpedia-org-search-api-openapi.yml
  format: yaml
  label: BLOBPEDIA Search API
  slug: blobpedia-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blobpedia-org/openapi/blobpedia-org-search-api-openapi.yml
auth_types: []
description: Authentication schemes published on the Celestia API authentication page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BLOBPEDIA Authentication
name_suffix: Authentication
oauth_flows: []
overview: BLOBPEDIA declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BLOBPEDIA
provider_slug: blobpedia-org
scheme_count: 1
schemes:
- evidence: 'Send the token in the Authorization header as a bearer token:'
  header: Authorization
  how_to_obtain: 'Generate a token on the node that serves the API, using the node type and --p2p.network value of the running node: celestia light auth admin --p2p.network mocha'
  location: header
  name: JWT
  type: http-bearer
slug: blobpedia-org-authentication
source_filename: blobpedia-org-authentication.yml
source_heading: Authentication Profile
source_url: https://blobpedia.org/docs/63866
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://blobpedia.org/docs/63866\nsources:\n- https://blobpedia.org/docs/63866\n- https://blobpedia.org/docs/96\n- https://blobpedia.org/docs/50\n- https://blobpedia.org/docs/224\ndescription: Authentication schemes published on the Celestia API authentication page.\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: 'Send the token in the Authorization header as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate a token on the node that serves the API, using the node type and --p2p.network value of the running node: celestia\n    light auth admin --p2p.network mocha'\ndocs: https://blobpedia.org/docs/63866\n"
source_yaml_url: https://artifacts.apis.io/blobpedia-org/authentication/blobpedia-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Celestia
- Knowledge Hub
- Documentation
- Community
- Open Source
---
