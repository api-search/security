---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mindmeister-com-files-api-openapi.yml
  format: yaml
  label: MindMeister Files API
  slug: mindmeister-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindmeister-com/openapi/mindmeister-com-files-api-openapi.yml
- filename: mindmeister-com-map-images-api-openapi.yml
  format: yaml
  label: MindMeister Map Images API
  slug: mindmeister-com-map-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindmeister-com/openapi/mindmeister-com-map-images-api-openapi.yml
- filename: mindmeister-com-maps-api-openapi.yml
  format: yaml
  label: MindMeister Maps API
  slug: mindmeister-com-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindmeister-com/openapi/mindmeister-com-maps-api-openapi.yml
- filename: mindmeister-com-user-preferences-api-openapi.yml
  format: yaml
  label: MindMeister User Preferences API
  slug: mindmeister-com-user-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindmeister-com/openapi/mindmeister-com-user-preferences-api-openapi.yml
- filename: mindmeister-com-users-api-openapi.yml
  format: yaml
  label: MindMeister Users API
  slug: mindmeister-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mindmeister-com/openapi/mindmeister-com-users-api-openapi.yml
auth_types: []
description: Authentication methods for MindMeister API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MindMeister Authentication
name_suffix: Authentication
oauth_flows: []
overview: MindMeister declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MindMeister
provider_slug: mindmeister-com
scheme_count: 2
schemes:
- authorize_url: https://www.mindmeister.com/oauth2/authorize
  evidence: The MindMeister API uses OAuth 2.0 for authorization.
  flows:
  - authorization_code
  - implicit
  - client_credentials
  how_to_obtain: Register an application to obtain a client_id and client_secret, then follow the appropriate OAuth 2.0 flow.
  name: OAuth 2.0
  type: oauth2
- evidence: Personal access tokens provide quick access to the MindMeister API.
  header: Authorization
  how_to_obtain: Create a personal access token via the MindMeister API page after logging in.
  name: Personal Access Token
  type: http-bearer
slug: mindmeister-com-authentication
source_filename: mindmeister-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.mindmeister.com/docs/oauth-2
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.mindmeister.com/docs/oauth-2\nsources:\n- https://developers.mindmeister.com/docs/oauth-2\n- https://developers.mindmeister.com/docs/oauth-20-endpoints\n- https://developers.mindmeister.com/docs/api-v1-with-oauth-20\n- https://developers.mindmeister.com/docs/personal-access-token\ndescription: Authentication methods for MindMeister API\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The MindMeister API uses OAuth 2.0 for authorization.\n  flows:\n  - authorization_code\n  - implicit\n  - client_credentials\n  authorize_url: https://www.mindmeister.com/oauth2/authorize\n  how_to_obtain: Register an application to obtain a client_id and client_secret, then follow the appropriate OAuth 2.0 flow.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Personal access tokens provide quick access to the MindMeister API.\n  header: Authorization\n\
  \  how_to_obtain: Create a personal access token via the MindMeister API page after logging in.\ndocs: https://developers.mindmeister.com/docs/oauth-2\n"
source_yaml_url: https://artifacts.apis.io/mindmeister-com/authentication/mindmeister-com-authentication.yml
summary_line: 2 schemes
tags:
- Mind Mapping
- Collaboration
- Productivity
- Artificial Intelligence
- Education
- Enterprise
---
