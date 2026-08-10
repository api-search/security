---
api_key_in:
- header
- query
auth_types:
- oauth2-device-code
- apiKey
- http-bearer
- anonymous
description: 'Kiota has no API of its own to authenticate against, so this profile covers the two authentication surfaces it genuinely publishes. (1) The CLI''s own sign-in to private API description repositories — `kiota login github device` (GitHub device code) or a personal access token. (2) The authentication model Kiota builds INTO the clients it generates: a required authentication provider on the request adapter, a set of built-in providers, and an allowed-hosts validator that keeps a token from being attached to an off-allowlist host. The second is the more consequential one — it is the auth posture every Kiota-generated SDK in the world inherits.'
kind: authentication
layout: security
method: searched
name: Kiota Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Kiota secures its APIs with oauth2-device-code, apiKey, http-bearer, and anonymous across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Kiota
provider_slug: kiota
scheme_count: 0
schemes: []
slug: kiota-authentication
source_filename: kiota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: >-\n  https://learn.microsoft.com/en-us/openapi/kiota/authentication and\n  https://github.com/microsoft/kiota/blob/main/specs/cli/login.md\ndocs: https://learn.microsoft.com/en-us/openapi/kiota/authentication\ndescription: >-\n  Kiota has no API of its own to authenticate against, so this profile covers the\n  two authentication surfaces it genuinely publishes. (1) The CLI's own sign-in to\n  private API description repositories — `kiota login github device` (GitHub\n  device code) or a personal access token. (2) The authentication model Kiota\n  builds INTO the clients it generates: a required authentication provider on the\n  request adapter, a set of built-in providers, and an allowed-hosts validator\n  that keeps a token from being attached to an off-allowlist host. The second is\n  the more consequential one — it is the auth posture every Kiota-generated SDK\n  in the world inherits.\nscope: cli-and-generated-clients\n\
  summary:\n  types: [oauth2-device-code, apiKey, http-bearer, anonymous]\n  api_key_in: [header, query]\n  oauth2_flows: [deviceCode]\n  design_note: >-\n    Kiota deliberately requires the authentication provider as a constructor\n    parameter on the request adapter rather than as an HTTP middleware handler, to\n    force the application developer to make a conscious choice about how the API\n    is authenticated.\ncli_authentication:\n  command: kiota login\n  purpose: >-\n    Sign in to private repositories so search, show and generate can reach private\n    API descriptions. `kiota logout` clears it.\n  providers:\n    - search_provider: github\n      strategies:\n        - id: device\n          type: oauth2-device-code\n          usage: kiota login github device\n        - id: pat\n          type: personal-access-token\n          usage: kiota login github pat --pat <value>\n          note: The PAT value is explicitly excluded from telemetry.\n  spec: https://github.com/microsoft/kiota/blob/main/specs/cli/login.md\n\
  generated_client_authentication:\n  interfaces:\n    - name: AuthenticationProvider\n      library: kiota abstractions\n      contract: >-\n        authenticateRequest(request, additionalAuthenticationContext) — completes\n        when the request object has been updated with authentication/authorization\n        information. Implemented per language (IAuthenticationProvider in .NET).\n    - name: AccessTokenProvider\n      library: kiota abstractions\n      contract: >-\n        getAuthorizationToken(uri, additionalAuthenticationContext) returns the\n        access token for the request URI, or null when the request should not be\n        authenticated; also exposes getAllowedHostsValidator().\n  providers:\n    - name: AnonymousAuthenticationProvider\n      type: anonymous\n      description: Placeholder that performs no operation, for APIs that require no authentication.\n    - name: ApiKeyAuthenticationProvider\n      type: apiKey\n      in: [header, query]\n      description: >-\n\
  \        Sets a named request header or query parameter to a supplied value.\n        Performs no encoding of the key or value — basic auth callers must\n        base64-encode \"userId:password\" before passing it in.\n    - name: BaseBearerTokenAuthenticationProvider\n      type: http\n      scheme: bearer\n      description: >-\n        Composes the Authorization bearer header from an AccessTokenProvider\n        implementation, so a new auth scheme only has to implement token\n        acquisition, not header composition.\n    - name: Microsoft Entra Identity authentication provider\n      type: oauth2\n      package: kiota authentication azure (Microsoft.Kiota.Authentication.Azure / microsoft-kiota-authentication-azure)\n      description: >-\n        Acquires access tokens from Microsoft Entra Identity and implements bearer\n        authentication; usable for any API secured by the Microsoft Entra Identity\n        Platform.\n  selection_guidance:\n    - condition: API requires no\
  \ authentication\n      use: AnonymousAuthenticationProvider\n    - condition: API is protected by Microsoft Identity Platform\n      use: Microsoft Entra Identity authentication provider\n    - condition: API uses an API key in a header or query parameter\n      use: ApiKeyAuthenticationProvider\n    - condition: API uses a bearer token in the Authorization header\n      use: Custom AccessTokenProvider with BaseBearerTokenAuthenticationProvider\n    - condition: Anything else\n      use: Custom AuthenticationProvider\n  security_controls:\n    - name: AllowedHostsValidator\n      description: >-\n        Validates the host of every request against an allowlist before the access\n        token provider returns a token. This is the control that stops a redirect\n        or a hostile server in a description from harvesting a caller's credential.\n    - name: --allowed-external-origins\n      added_in: 1.32.5\n      description: >-\n        External $refs in an OpenAPI description are no\
  \ longer resolved by default;\n        this parameter opts specific origins, URIs, patterns or paths back in.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n    - url: https://learn.microsoft.com/en-us/openapi/kiota/authentication\n      status: 200\n    - url: https://raw.githubusercontent.com/microsoft/kiota/main/specs/cli/login.md\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiota/refs/heads/main/authentication/kiota-authentication.yml
summary_line: oauth2-device-code/apiKey/http-bearer/anonymous · 0 schemes
tags:
- Code Generation
- Microsoft
- OpenAPI
- SDKs
- Developer Tools
- API Clients
- Open Source
- CLI
- JSON Schema
---
