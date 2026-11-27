---
anonymous_access: true
api_key_in: []
auth_types: []
description: Kubb publishes no HTTP API contract for Kubb Studio. The documented credentials are those the kubb CLI and git use against kubb.studio; the Kubb Extension Registry (https://kubb.dev/registry) is public static JSON with no authentication.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Kubb Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kubb Studio declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Kubb Studio
provider_slug: kubb-studio
scheme_count: 4
schemes:
- description: kubb studio shows a pairing code that a user approves in the Studio window; the CLI then stores a per-project token (forgotten by kubb studio logout). The Docker agent is approved by an organization admin.
  name: device-pairing
  source: https://kubb.dev/docs/5.x/reference/commands/studio
  type: pairing-code
- description: Organization CI API key used only by kubb studio snapshot.
  in: cli-flag / environment
  name: organization-ci-api-key
  parameter: KUBB_TOKEN (or --token=<key>)
  source: https://kubb.dev/docs/5.x/reference/commands
  type: apiKey
- description: Token of type AI (read-only), created under Settings › Developers › Tokens, used as the git password for the plugin marketplace at https://kubb.studio/plugins/<organization-slug>.git; any username works. A registry key does not work here. Pro plan.
  name: ai-key
  scheme: basic
  source: https://kubb.dev/docs/5.x/integrations/studio
  type: http
- description: Registry documents are served as application/json with CORS allowed and no authentication.
  name: registry-public
  source: https://kubb.dev/docs/5.x/reference/registry
  type: none
slug: kubb-studio-authentication
source_filename: kubb-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: searched\nsource: https://kubb.dev/docs/5.x/reference/commands/studio\ndocs: https://kubb.dev/docs/5.x/integrations/studio\ndescription: Kubb publishes no HTTP API contract for Kubb Studio. The documented credentials are those the kubb CLI and git use against kubb.studio; the Kubb Extension Registry (https://kubb.dev/registry)\n  is public static JSON with no authentication.\nschemes:\n- name: device-pairing\n  type: pairing-code\n  description: kubb studio shows a pairing code that a user approves in the Studio window; the CLI then stores a per-project token (forgotten by kubb studio logout). The Docker agent is approved by an organization\n    admin.\n  source: https://kubb.dev/docs/5.x/reference/commands/studio\n- name: organization-ci-api-key\n  type: apiKey\n  in: cli-flag / environment\n  parameter: KUBB_TOKEN (or --token=<key>)\n  description: Organization CI API key used only by kubb studio snapshot.\n  source: https://kubb.dev/docs/5.x/reference/commands\n\
  - name: ai-key\n  type: http\n  scheme: basic\n  description: Token of type AI (read-only), created under Settings › Developers › Tokens, used as the git password for the plugin marketplace at https://kubb.studio/plugins/<organization-slug>.git; any\n    username works. A registry key does not work here. Pro plan.\n  source: https://kubb.dev/docs/5.x/integrations/studio\n- name: registry-public\n  type: none\n  description: Registry documents are served as application/json with CORS allowed and no authentication.\n  source: https://kubb.dev/docs/5.x/reference/registry\n"
source_yaml_url: https://artifacts.apis.io/kubb-studio/authentication/kubb-studio-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Code Generation
- OpenAPI
- TypeScript
- SDK Generation
- Developer Tools
- API Client
- Zod
- TanStack Query
- Mocking
---
