---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dynaboard-openapi-generated.yml
  format: yaml
  label: Dynaboard API
  slug: dynaboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynaboard/openapi/_ae-authored/dynaboard-openapi-generated.yml
auth_types: []
description: Authentication schemes for Dynaboard OAuth resources
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Dynaboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynaboard declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Dynaboard
provider_slug: dynaboard
scheme_count: 4
schemes:
- evidence: The Facebook Authentication Resource authenticates with the Facebook OAuth 2 API.
  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).
  name: Facebook Authentication
  type: oauth2
- evidence: The GitHub Authentication Resource authenticates with the GitHub OAuth 2 API.
  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).
  name: GitHub Authentication
  type: oauth2
- evidence: The Google Authentication Resource authenticates with the Google OAuth 2 API.
  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).
  name: Google Authentication
  type: oauth2
- evidence: The Microsoft Authentication Resource authenticates with the Microsoft OAuth 2 API.
  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).
  name: Microsoft Authentication
  type: oauth2
slug: dynaboard-authentication
source_filename: dynaboard-authentication.yml
source_heading: Authentication Profile
source_url: https://dynaboard.com/docs/reference/nodes/resources/facebook-authentication
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dynaboard.com/docs/reference/nodes/resources/facebook-authentication\nsources:\n- https://dynaboard.com/docs/reference/nodes/resources/facebook-authentication\n- https://dynaboard.com/docs/reference/nodes/resources/github-authentication\n- https://dynaboard.com/docs/reference/nodes/resources/google-authentication\n- https://dynaboard.com/docs/reference/nodes/resources/microsoft-authentication\ndescription: Authentication schemes for Dynaboard OAuth resources\nschemes:\n- type: oauth2\n  name: Facebook Authentication\n  evidence: The Facebook Authentication Resource authenticates with the Facebook OAuth 2 API.\n  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).\n- type: oauth2\n  name: GitHub Authentication\n  evidence: The GitHub Authentication Resource authenticates with the GitHub OAuth 2 API.\n\
  \  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).\n- type: oauth2\n  name: Google Authentication\n  evidence: The Google Authentication Resource authenticates with the Google OAuth 2 API.\n  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).\n- type: oauth2\n  name: Microsoft Authentication\n  evidence: The Microsoft Authentication Resource authenticates with the Microsoft OAuth 2 API.\n  how_to_obtain: Provide a Client ID and Client Secret in the resource's Environment Profile properties (clientID, clientSecret).\ndocs: https://dynaboard.com/docs/reference/nodes/resources/facebook-authentication\n"
source_yaml_url: https://artifacts.apis.io/dynaboard/authentication/dynaboard-authentication.yml
summary_line: 4 schemes
tags:
- Low-code
- Collaboration
- Real-time
- AI
- Web Development
---
