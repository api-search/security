---
anonymous_access: false
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
mechanism_count: 6
method: searched
name: Kiota Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Kiota secures its APIs with oauth2-device-code, apiKey, http-bearer, and anonymous across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Kiota
provider_slug: kiota
scheme_count: 6
schemes:
- name: kiota login github device
  surface: cli
  type: oauth2-device-code
  usage: kiota login github device
- name: kiota login github pat
  surface: cli
  type: personal-access-token
  usage: kiota login github pat --pat <value>
- name: AnonymousAuthenticationProvider
  surface: generated-client
  type: anonymous
- in:
  - header
  - query
  name: ApiKeyAuthenticationProvider
  surface: generated-client
  type: apiKey
- name: BaseBearerTokenAuthenticationProvider
  scheme: bearer
  surface: generated-client
  type: http
- name: Microsoft Entra Identity authentication provider
  surface: generated-client
  type: oauth2
slug: kiota-authentication
source_filename: kiota-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/openapi/kiota/authentication and https://github.com/microsoft/kiota/blob/main/specs/cli/login.md\ndocs: https://learn.microsoft.com/en-us/openapi/kiota/authentication\ndescription: 'Kiota has no API of its own to authenticate against, so this profile covers the two authentication surfaces it genuinely publishes. (1) The CLI''s own sign-in to private API description repositories\n  — `kiota login github device` (GitHub device code) or a personal access token. (2) The authentication model Kiota builds INTO the clients it generates: a required authentication provider on the request\n  adapter, a set of built-in providers, and an allowed-hosts validator that keeps a token from being attached to an off-allowlist host. The second is the more consequential one — it is the auth posture\n  every Kiota-generated SDK in the world inherits.'\nscope: cli-and-generated-clients\nsummary:\n  types:\n  - oauth2-device-code\n\
  \  - apiKey\n  - http-bearer\n  - anonymous\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - deviceCode\n  design_note: Kiota deliberately requires the authentication provider as a constructor parameter on the request adapter rather than as an HTTP middleware handler, to force the application developer to\n    make a conscious choice about how the API is authenticated.\ncli_authentication:\n  command: kiota login\n  purpose: Sign in to private repositories so search, show and generate can reach private API descriptions. `kiota logout` clears it.\n  providers:\n  - search_provider: github\n    strategies:\n    - id: device\n      type: oauth2-device-code\n      usage: kiota login github device\n    - id: pat\n      type: personal-access-token\n      usage: kiota login github pat --pat <value>\n      note: The PAT value is explicitly excluded from telemetry.\n  spec: https://github.com/microsoft/kiota/blob/main/specs/cli/login.md\ngenerated_client_authentication:\n  interfaces:\n\
  \  - name: AuthenticationProvider\n    library: kiota abstractions\n    contract: authenticateRequest(request, additionalAuthenticationContext) — completes when the request object has been updated with authentication/authorization information. Implemented per language (IAuthenticationProvider\n      in .NET).\n  - name: AccessTokenProvider\n    library: kiota abstractions\n    contract: getAuthorizationToken(uri, additionalAuthenticationContext) returns the access token for the request URI, or null when the request should not be authenticated; also exposes getAllowedHostsValidator().\n  providers:\n  - name: AnonymousAuthenticationProvider\n    type: anonymous\n    description: Placeholder that performs no operation, for APIs that require no authentication.\n  - name: ApiKeyAuthenticationProvider\n    type: apiKey\n    in: &id001\n    - header\n    - query\n    description: Sets a named request header or query parameter to a supplied value. Performs no encoding of the key or value — basic\
  \ auth callers must base64-encode \"userId:password\" before passing it\n      in.\n  - name: BaseBearerTokenAuthenticationProvider\n    type: http\n    scheme: bearer\n    description: Composes the Authorization bearer header from an AccessTokenProvider implementation, so a new auth scheme only has to implement token acquisition, not header composition.\n  - name: Microsoft Entra Identity authentication provider\n    type: oauth2\n    package: kiota authentication azure (Microsoft.Kiota.Authentication.Azure / microsoft-kiota-authentication-azure)\n    description: Acquires access tokens from Microsoft Entra Identity and implements bearer authentication; usable for any API secured by the Microsoft Entra Identity Platform.\n  selection_guidance:\n  - condition: API requires no authentication\n    use: AnonymousAuthenticationProvider\n  - condition: API is protected by Microsoft Identity Platform\n    use: Microsoft Entra Identity authentication provider\n  - condition: API uses an API key\
  \ in a header or query parameter\n    use: ApiKeyAuthenticationProvider\n  - condition: API uses a bearer token in the Authorization header\n    use: Custom AccessTokenProvider with BaseBearerTokenAuthenticationProvider\n  - condition: Anything else\n    use: Custom AuthenticationProvider\n  security_controls:\n  - name: AllowedHostsValidator\n    description: Validates the host of every request against an allowlist before the access token provider returns a token. This is the control that stops a redirect or a hostile server in a description\n      from harvesting a caller's credential.\n  - name: --allowed-external-origins\n    added_in: 1.32.5\n    description: External $refs in an OpenAPI description are no longer resolved by default; this parameter opts specific origins, URIs, patterns or paths back in.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://learn.microsoft.com/en-us/openapi/kiota/authentication\n    status: 200\n  - url: https://raw.githubusercontent.com/microsoft/kiota/main/specs/cli/login.md\n\
  \    status: 200\nschemes:\n- name: kiota login github device\n  type: oauth2-device-code\n  surface: cli\n  usage: kiota login github device\n- name: kiota login github pat\n  type: personal-access-token\n  surface: cli\n  usage: kiota login github pat --pat <value>\n- name: AnonymousAuthenticationProvider\n  type: anonymous\n  surface: generated-client\n- name: ApiKeyAuthenticationProvider\n  type: apiKey\n  surface: generated-client\n  in: *id001\n- name: BaseBearerTokenAuthenticationProvider\n  type: http\n  surface: generated-client\n  scheme: bearer\n- name: Microsoft Entra Identity authentication provider\n  type: oauth2\n  surface: generated-client\n"
source_yaml_url: https://artifacts.apis.io/kiota/authentication/kiota-authentication.yml
summary_line: oauth2-device-code/apiKey/http-bearer/anonymous · 6 schemes
tags:
- Code Generation
- Microsoft
- OpenAPI
- SDK
- Developer Tools
- API Client
- Open Source
- CLI
- JSON Schema
- SDK Generation
---
