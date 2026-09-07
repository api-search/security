---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Intlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intlayer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Intlayer
provider_slug: intlayer
scheme_count: 1
schemes:
- bearer_method: header
  deviations:
  - 'The token response is wrapped in Intlayer''s standard envelope ({ "data": { ... } }) rather than returned as a bare RFC 6749 token response — clients must read data.accessToken. The provider documents this deviation itself in auth.md.'
  flow: client_credentials
  registration: No dynamic client registration — credentials are issued per project by a human account holder at https://app.intlayer.org/projects (client ID + client secret, secret shown once).
  scopes: None — authorization is governed by the role attached to the access key, optionally restricted to specific environments and locales, not by requested OAuth scopes.
  token_endpoint: https://back.intlayer.org/oauth2/token
  token_endpoint_auth_method: client_secret_post
  token_extend_endpoint: https://back.intlayer.org/oauth2/token/extend
  token_lifetime_seconds: 604800
  type: oauth2
slug: intlayer-authentication
source_filename: intlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://intlayer.org/auth.md\ndocs: https://intlayer.org/doc/concept/cms\nnote: >-\n  Intlayer publishes a machine-readable authentication guide for AI agents at\n  https://intlayer.org/auth.md (saved verbatim at skills/intlayer-auth.md), and RFC 8414\n  authorization-server metadata plus RFC 9728 protected-resource metadata on\n  back.intlayer.org (saved under well-known/). No OpenAPI exists, so this profile is written\n  from those provider-published documents rather than derived from securitySchemes.\nresource: https://back.intlayer.org\nauthorization_server_metadata: https://back.intlayer.org/.well-known/oauth-authorization-server\nprotected_resource_metadata: https://back.intlayer.org/.well-known/oauth-protected-resource\nschemes:\n- type: oauth2\n  flow: client_credentials\n  token_endpoint: https://back.intlayer.org/oauth2/token\n  token_extend_endpoint: https://back.intlayer.org/oauth2/token/extend\n  token_endpoint_auth_method:\
  \ client_secret_post\n  token_lifetime_seconds: 604800\n  bearer_method: header\n  registration: >-\n    No dynamic client registration — credentials are issued per project by a human account\n    holder at https://app.intlayer.org/projects (client ID + client secret, secret shown once).\n  scopes: >-\n    None — authorization is governed by the role attached to the access key, optionally\n    restricted to specific environments and locales, not by requested OAuth scopes.\n  deviations:\n  - >-\n    The token response is wrapped in Intlayer's standard envelope ({ \"data\": { ... } }) rather\n    than returned as a bare RFC 6749 token response — clients must read data.accessToken. The\n    provider documents this deviation itself in auth.md.\nagent_auth:\n  note: >-\n    The authorization-server metadata carries a non-standard agent_auth block aimed at\n    autonomous agents: skill https://intlayer.org/auth.md, manual registration at\n    https://app.intlayer.org/projects, identity type\
  \ \"project\", credential type\n    client_credentials, token lifetime 604800 seconds.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intlayer/refs/heads/main/authentication/intlayer-authentication.yml
summary_line: 1 scheme
tags:
- i18n
- Internationalization
- Localization
- React
- Next.js
- CMS
- MCP
---
