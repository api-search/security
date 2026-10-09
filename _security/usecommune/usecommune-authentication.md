---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usecommune-articles-api-openapi.yml
  format: yaml
  label: Commune Articles API
  slug: usecommune-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-articles-api-openapi.yml
- filename: usecommune-engagement-api-openapi.yml
  format: yaml
  label: Commune Engagement API
  slug: usecommune-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-engagement-api-openapi.yml
- filename: usecommune-event-delivery-api-openapi.yml
  format: yaml
  label: Commune Event delivery API
  slug: usecommune-event-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-event-delivery-api-openapi.yml
- filename: usecommune-highlights-api-openapi.yml
  format: yaml
  label: Commune Highlights API
  slug: usecommune-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-highlights-api-openapi.yml
- filename: usecommune-messages-api-openapi.yml
  format: yaml
  label: Commune Messages API
  slug: usecommune-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-messages-api-openapi.yml
- filename: usecommune-metrics-api-openapi.yml
  format: yaml
  label: Commune Metrics API
  slug: usecommune-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-metrics-api-openapi.yml
- filename: usecommune-newsletters-api-openapi.yml
  format: yaml
  label: Commune Newsletters API
  slug: usecommune-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-newsletters-api-openapi.yml
- filename: usecommune-platform-api-openapi.yml
  format: yaml
  label: Commune Platform API
  slug: usecommune-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-platform-api-openapi.yml
- filename: usecommune-search-api-openapi.yml
  format: yaml
  label: Commune Search API
  slug: usecommune-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-search-api-openapi.yml
- filename: usecommune-senders-api-openapi.yml
  format: yaml
  label: Commune Senders API
  slug: usecommune-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-senders-api-openapi.yml
- filename: usecommune-sends-api-openapi.yml
  format: yaml
  label: Commune Sends API
  slug: usecommune-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-sends-api-openapi.yml
- filename: usecommune-subscriber-tags-api-openapi.yml
  format: yaml
  label: Commune Subscriber tags API
  slug: usecommune-subscriber-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscriber-tags-api-openapi.yml
- filename: usecommune-subscribers-api-openapi.yml
  format: yaml
  label: Commune Subscribers API
  slug: usecommune-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscribers-api-openapi.yml
- filename: usecommune-team-api-openapi.yml
  format: yaml
  label: Commune Team API
  slug: usecommune-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-team-api-openapi.yml
- filename: usecommune-threads-api-openapi.yml
  format: yaml
  label: Commune Threads API
  slug: usecommune-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-threads-api-openapi.yml
- filename: usecommune-users-api-openapi.yml
  format: yaml
  label: Commune Users API
  slug: usecommune-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-users-api-openapi.yml
- filename: usecommune-webhooks-api-openapi.yml
  format: yaml
  label: Commune Webhooks API
  slug: usecommune-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-webhooks-api-openapi.yml
- filename: usecommune-website-domains-api-openapi.yml
  format: yaml
  label: Commune Website domains API
  slug: usecommune-website-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-website-domains-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Usecommune Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Commune secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Commune
provider_slug: usecommune
scheme_count: 2
schemes:
- description: 'An OAuth access token, sent as `Authorization: Bearer <token>`. The

    walkthrough of the whole flow is at

    [usecommune.dev/use-cases/build-an-integration](https://usecommune.dev/use-cases/build-an-integration):

    discovery, registration, PKCE, the consent screen, the exchange, refresh

    and revocation.


    Ask for a family scope and the person picks which newsletter

    the token reaches; ask for `account:read`'
  flows:
  - authorizationUrl: https://usecommune.com/api/oauth/authorize
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://usecommune.com/api/oauth/token
  name: oauth2
  sources:
  - openapi/usecommune-openapi.yml
  type: oauth2
- bearerFormat: Commune API key
  description: 'A Commune API key, sent as `Authorization: Bearer <key>`. A key is

    granted one or more newsletters and carries six permission families on

    each, every one of them `none`, `read` or `write`. An operation names

    the family and the level it needs.


    A key is minted by a creator in Commune''s settings: no flow, no consent

    screen, no expiry. That is the whole difference from `oauth2`. An

    operation that dec'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/usecommune-openapi.yml
  type: http
slug: usecommune-authentication
source_filename: usecommune-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: openapi/usecommune-openapi.yml; https://usecommune.dev/use-cases/build-an-integration; https://usecommune.dev/guides/getting-started;\n  https://api.usecommune.com/.well-known/oauth-protected-resource; https://usecommune.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usecommune.com/api/oauth/authorize\n    tokenUrl: https://usecommune.com/api/oauth/token\n    scopes: 13\n  description: 'An OAuth access token, sent as `Authorization: Bearer <token>`. The\n\n    walkthrough of the whole flow is at\n\n    [usecommune.dev/use-cases/build-an-integration](https://usecommune.dev/use-cases/build-an-integration):\n\n    discovery, registration, PKCE, the consent screen, the exchange, refresh\n\n    and revocation.\n\n\n    Ask for a family scope\
  \ and the person picks which newsletter\n\n    the token reaches; ask for `account:read`'\n  sources:\n  - openapi/usecommune-openapi.yml\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: Commune API key\n  description: 'A Commune API key, sent as `Authorization: Bearer <key>`. A key is\n\n    granted one or more newsletters and carries six permission families on\n\n    each, every one of them `none`, `read` or `write`. An operation names\n\n    the family and the level it needs.\n\n\n    A key is minted by a creator in Commune''s settings: no flow, no consent\n\n    screen, no expiry. That is the whole difference from `oauth2`. An\n\n    operation that dec'\n  sources:\n  - openapi/usecommune-openapi.yml\ndocs: https://usecommune.dev/use-cases/build-an-integration\ndiscovery:\n  rfc9728_protected_resource: https://api.usecommune.com/.well-known/oauth-protected-resource (200)\n  rfc8414_authorization_server: https://usecommune.com/.well-known/oauth-authorization-server (200)\n\
  \  www_authenticate_on_401: Bearer realm=\"Commune API\", resource_metadata=\"https://api.usecommune.com/.well-known/oauth-protected-resource\"\n  dynamic_client_registration: https://usecommune.com/api/oauth/register (RFC 7591, token_endpoint_auth_method none\n    supported)\n  pkce: S256 required for public clients\n  refresh: refresh_token grant; offline_access scope\napi_keys:\n  prefix: cmn_sk_\n  minted_at: https://usecommune.com/settings/api-keys\n  expiry: none; revocable via DELETE /api-keys/{key} or in settings\n  grant: per newsletter, six families each none/read/write, plus optional account:read\npermission_model:\n  families:\n  - content\n  - audience\n  - sending\n  - insights\n  - settings\n  - webhooks\n  levels:\n  - none\n  - read\n  - write\n  separate_axis: account:read\n  enforcement: 403 forbidden / insufficient_scope naming what was needed and what the credential holds\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/authentication/usecommune-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Newsletters
- Email
- Community
- Publishing
- Creator Economy
- Subscribers
- Webhooks
- MCP
- Analytics
- Content
---
