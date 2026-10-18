---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes as published on the GitLab documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Media2Url Authentication
name_suffix: Authentication
oauth_flows: []
overview: Media2URL Direct Media Delivery API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Media2URL Direct Media Delivery API
provider_slug: media2url
scheme_count: 1
schemes:
- authorize_url: https://gitlab.example.com/oauth/authorize
  evidence: 'GitLab supports the following authorization flows: Authorization code with Proof Key for Code Exchange (PKCE) :'
  flows:
  - authorization_code
  - authorization_code_pkce
  how_to_obtain: Register an application via the /user_settings/applications page to obtain an Application ID and Client Secret.
  name: GitLab OAuth2
  type: oauth2
slug: media2url-authentication
source_filename: media2url-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.gitlab.com/auth/
source_yaml: "generated: '2026-10-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.gitlab.com/auth/\nsources:\n- https://docs.gitlab.com/auth/\n- https://docs.gitlab.com/auth/user_authentication/\n- https://docs.gitlab.com/user/duo_agent_platform/authentication/\n- https://docs.gitlab.com/api/oauth2/\ndescription: Authentication schemes as published on the GitLab documentation pages.\nschemes:\n- type: oauth2\n  name: GitLab OAuth2\n  evidence: 'GitLab supports the following authorization flows: Authorization code with Proof Key for Code Exchange (PKCE) :'\n  flows:\n  - authorization_code\n  - authorization_code_pkce\n  authorize_url: https://gitlab.example.com/oauth/authorize\n  how_to_obtain: Register an application via the /user_settings/applications page to obtain an Application ID and Client Secret.\ndocs: https://docs.gitlab.com/auth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/media2url/refs/heads/main/authentication/media2url-authentication.yml
summary_line: 1 scheme
tags:
- Media
- FileHosting
- DirectLinks
- Upload
---
