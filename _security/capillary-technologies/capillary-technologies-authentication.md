---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capillary-technologies-events-api-openapi.yml
  format: yaml
  label: Capillary Technologies Events API
  slug: capillary-technologies-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-events-api-openapi.yml
- filename: capillary-technologies-simulation-api-openapi.yml
  format: yaml
  label: Capillary Technologies Simulation API
  slug: capillary-technologies-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-simulation-api-openapi.yml
- filename: capillary-technologies-webhooks-api-openapi.yml
  format: yaml
  label: Capillary Technologies Webhooks API
  slug: capillary-technologies-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-webhooks-api-openapi.yml
- filename: capillary-technologies-x-api-openapi.yml
  format: yaml
  label: Capillary Technologies X API
  slug: capillary-technologies-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-x-api-openapi.yml
auth_types: []
description: Authentication methods documented for Capillary Technologies
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Capillary Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capillary Technologies declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Capillary Technologies
provider_slug: capillary-technologies
scheme_count: 1
schemes:
- evidence: In basic authentication, the till ID and password (in MD5 format) are used for authenticating the APIs.
  header: Authorization
  how_to_obtain: Create till credentials in the Capillary UI (Add till) and enable basic authentication via a support ticket; then construct the Authorization header as `Basic <Base64 encoded (username:md5(password))>`.
  location: header
  name: Basic Authentication
  type: http-basic
slug: capillary-technologies-authentication
source_filename: capillary-technologies-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.capillarytech.com/docs/connect-to-destination-block-without-oauth-authentication.md
source_yaml: "generated: '2026-10-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.capillarytech.com/docs/connect-to-destination-block-without-oauth-authentication.md\nsources:\n- https://docs.capillarytech.com/docs/connect-to-destination-block-without-oauth-authentication.md\n- https://docs.capillarytech.com/docs/capillarys-oauth-block.md\n- https://docs.capillarytech.com/docs/api-client.md\n- https://docs.capillarytech.com/docs/basic-authentication-api.md\ndescription: Authentication methods documented for Capillary Technologies\nschemes:\n- type: http-basic\n  name: Basic Authentication\n  evidence: In basic authentication, the till ID and password (in MD5 format) are used for authenticating the APIs.\n  location: header\n  header: Authorization\n  how_to_obtain: Create till credentials in the Capillary UI (Add till) and enable basic authentication via a support ticket; then construct the\n    Authorization header as `Basic <Base64 encoded (username:md5(password))>`.\n\
  docs: https://docs.capillarytech.com/docs/connect-to-destination-block-without-oauth-authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/authentication/capillary-technologies-authentication.yml
summary_line: 1 scheme
tags:
- Loyalty
- Marketing
- Software-as-a-Service
- Enterprise
- Customer-Engagement
---
