---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Publicis Groupe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Publicis Groupe declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Publicis Groupe
provider_slug: publicis-groupe
scheme_count: 0
schemes: []
slug: publicis-groupe-authentication
source_filename: publicis-groupe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  PublicisSapient/knowhow-api src/main/java/com/publicissapient/kpidashboard/apis/config/OpenApiConfig.java\n  (first-party source) and the @psnext/slingcli and @psnext/block-sdk package READMEs, read 2026-09-13\nname: Publicis Groupe — authentication profile\nnote: >-\n  Derived from first-party source and published package documentation rather than from a\n  captured OpenAPI, because the KnowHOW spec is generated at runtime on a self-hosted\n  instance and no public deployment exists to fetch it from. Each scheme below is quoted\n  from the code or docs that define it.\napis:\n- api: publicis-groupe-knowhow\n  name: Publicis Sapient KnowHOW\n  source: >-\n    OpenApiConfig.java declares both schemes and applies them as top-level security\n    requirements on the generated OpenAPI document.\n  security_schemes:\n  - key: cookieAuth\n    type: apiKey\n    in: cookie\n    name: authCookie\n    description: Session cookie\
  \ issued by the KnowHOW auth service after interactive login.\n  - key: apiKeyAuth\n    type: apiKey\n    in: header\n    name: x-api-key\n    description: Static API key header for machine-to-machine calls against a KnowHOW deployment.\n  applied: both schemes are added as OpenAPI securityItems, so they apply document-wide\n  oauth2: false\n  scopes: none — neither scheme carries a scope model\n- api: publicis-groupe-sapient-slingshot\n  name: Sapient Slingshot\n  source: '@psnext/slingcli README: \"First-time login\" and \"Environment variables\"'\n  security_schemes:\n  - key: slingshotOAuth\n    type: oauth2\n    flow: authorization_code (browser)\n    description: >-\n      `/login slingshot` inside the sling TUI opens a browser window and completes an\n      interactive login against Slingshot. The authorization server, token endpoint and\n      scopes are not published; no /.well-known/oauth-authorization-server document is\n      served on any Publicis host probed.\n  - key: slingshotToken\n\
  \    type: http\n    scheme: bearer\n    env: SLINGSHOT_TOKEN\n    description: >-\n      A pre-issued Slingshot access token supplied via the SLINGSHOT_TOKEN environment\n      variable, which bypasses the interactive login.\n- api: coreai-blocks\n  name: CoreAI Block SDK\n  source: '@psnext/block-sdk README: Fetcher and register()'\n  security_schemes:\n  - key: coreaiBlockToken\n    type: platform-managed\n    description: >-\n      Blocks authenticate through the SDK's register() call; the Fetcher utility carries\n      integrated CoreAI authentication with token validation and automatic refresh. Token\n      format, issuer and lifetime are not published.\nobservations:\n  self_service_signup: false\n  public_token_issuance: false\n  discovery_documents_served: none\n  note: >-\n    Nothing in the Groupe's public surface issues credentials to an unaffiliated developer.\n    KnowHOW keys are minted inside an operator's own deployment; Slingshot and CoreAI\n    credentials are issued\
  \ to Publicis employees and clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publicis-groupe/refs/heads/main/authentication/publicis-groupe-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- Marketing
- Media
- Digital Transformation
- Consulting
- Artificial Intelligence
- Developer Tools
- Engineering Metrics
- Open-Source
- MCP
- Agency Holding Company
---
