---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tabnine-groups-api-openapi.yml
  format: yaml
  label: Tabnine Groups API
  slug: tabnine-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/openapi/tabnine-groups-api-openapi.yml
- filename: tabnine-main-api-openapi.yml
  format: yaml
  label: Tabnine Main API
  slug: tabnine-main-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/openapi/tabnine-main-api-openapi.yml
- filename: tabnine-schemas-api-openapi.yml
  format: yaml
  label: Tabnine Schemas API
  slug: tabnine-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/openapi/tabnine-schemas-api-openapi.yml
- filename: tabnine-users-api-openapi.yml
  format: yaml
  label: Tabnine Users API
  slug: tabnine-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/openapi/tabnine-users-api-openapi.yml
auth_types: []
description: Authentication methods documented for Tabnine
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tabnine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabnine declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tabnine
provider_slug: tabnine
scheme_count: 1
schemes:
- evidence: Include the PAT as a bearer token in the Authorization header of your HTTP requests.
  header: Authorization
  how_to_obtain: Generate a PAT in the Admin Console under Settings → Access Tokens, copy the token value (it will not be shown again).
  location: header
  name: Personal Access Token
  type: http-bearer
slug: tabnine-authentication
source_filename: tabnine-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tabnine.com/main/getting-started/install/client-setup-private-installation/sign-in-using-authentication-token.md
source_yaml: "generated: '2026-10-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tabnine.com/main/getting-started/install/client-setup-private-installation/sign-in-using-authentication-token.md\nsources:\n- https://docs.tabnine.com/main/getting-started/install/client-setup-private-installation/sign-in-using-authentication-token.md\n- https://docs.tabnine.com/main/administering-tabnine/managing-your-team/user-management/service-accounts-and-token-limits.md\n- https://docs.tabnine.com/main/administering-tabnine/managing-your-team/settings/access-tokens.md\n- https://docs.tabnine.com/main/getting-started/install.md\ndescription: Authentication methods documented for Tabnine\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Include the PAT as a bearer token in the Authorization header of your HTTP requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a PAT in the Admin Console under Settings → Access\
  \ Tokens, copy the token value (it will not be shown again).\ndocs: https://docs.tabnine.com/main/getting-started/install/client-setup-private-installation/sign-in-using-authentication-token.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabnine/refs/heads/main/authentication/tabnine-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Developer Tools
- Code Completion
- Self-Hosted
- Enterprise
- Privacy
---
