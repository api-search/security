---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Verily Life Sciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Verily Life Sciences declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Verily Life Sciences
provider_slug: verily-life-sciences
scheme_count: 0
schemes: []
slug: verily-life-sciences-authentication
source_filename: verily-life-sciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://support.workbench.verily.com/docs/references/cli_reference/wb/auth/, https://github.com/verily-src/terraform-provider-workbench\ndocs: https://support.workbench.verily.com/docs/references/cli_reference/wb/auth/\nname: Verily Workbench — authentication profile\nsummary: >-\n  Verily Workbench delegates identity entirely to Google. There is no Workbench-issued API key, no\n  Workbench developer console that mints credentials, and no self-serve token page. Every caller\n  authenticates as a Google identity (Gmail or Google Workspace) or as an impersonated Google service\n  account, and presents the resulting token as a bearer token to the control-plane API. This profile is\n  assembled from the CLI reference and from Verily's own open-source Terraform provider, whose generated\n  clients name the security schemes the API declares; it is NOT derived from a published OpenAPI, because\n  Verily serves none publicly (the spec\
  \ endpoints return HTTP 403).\napi_base: https://workbench.verily.com/api\nsecurity_schemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: Google OAuth 2.0 access token or Google-signed ID token\n  evidence: >-\n    Declared as `BearerAuthScopes = \"bearerAuth.Scopes\"` in the oapi-codegen generated clients at\n    internal/openapi/wsm/types.go and internal/openapi/user/types.go in\n    github.com/verily-src/terraform-provider-workbench — code generated from Verily's internal OpenAPI.\n  applies_to: [/api/wsm, /api/user]\n- name: authorization\n  type: apiKey\n  in: header\n  header: Authorization\n  evidence: >-\n    Declared as `AuthorizationScopes = \"authorization.Scopes\"` in the same generated clients. Recorded as\n    published; the exact distinction from bearerAuth is not documented publicly.\n  applies_to: [/api/wsm, /api/user]\nidentity_providers:\n- provider: Google (Gmail / Google Workspace)\n  note: >-\n    \"Self-serve account creation via Gmail or\
  \ Google identity\" is the documented path onto the free\n    Standard tier.\n  source: https://verily.com/newsroom/verily-launches-free-version-of-its-pre-exchange-and-workbench-solutions-powering-precision-health-ai-and-discovery\n- provider: Google Cloud service account (impersonation)\n  note: >-\n    The Terraform provider exposes `impersonate_service_account` (a service-account email impersonated via\n    Application Default Credentials) and `use_id_token` (send a Google ID token rather than an access\n    token; documented as false for local development).\n  source: https://github.com/verily-src/terraform-provider-workbench/blob/main/docs/index.md\nclient_flows:\n- client: wb CLI\n  commands:\n  - command: wb auth login\n    note: Interactive browser-based Google login.\n  - command: wb auth status\n    note: Reports the currently authenticated identity.\n  - command: wb auth print-access-token\n    note: Prints the bearer token the CLI holds — the documented way to call the REST\
  \ API directly.\n  - command: wb auth revoke\n    note: Revokes the stored credential.\n  prerequisite: gcloud SDK installed (documented CLI prerequisite).\n- client: Terraform provider verily-src/workbench\n  configuration:\n    host: https://workbench.verily.com\n    impersonate_service_account: <service account email>\n    use_id_token: true\n- client: SSH keys\n  note: >-\n    Separate from API authentication. `wb security ssh-key generate|add|get` manages keys used to reach\n    workspace compute, not the control-plane API.\nscopes:\n  documented: false\n  note: >-\n    No OAuth scope reference page is published, and the spec endpoints that would carry the scope names\n    are 403. `scopes/` is therefore not emitted rather than being filled with guesses.\npublic_unauthenticated_endpoints:\n- url: https://workbench.verily.com/api/axon/cli-version\n  status: 200\n  note: Returns supported CLI version window and artifact checksum.\n- url: https://workbench.verily.com/api/wsm/version\n\
  \  status: 200\n- url: https://workbench.verily.com/api/axon/version\n  status: 200\n- url: https://workbench.verily.com/api/user/version\n  status: 200\n- url: https://workbench.verily.com/api/wsm/status\n  status: 200\n- url: https://workbench.verily.com/api/axon/status\n  status: 200\n- url: https://workbench.verily.com/api/user/status\n  status: 200\ngaps:\n- No published OAuth scope list.\n- No API-key or personal-access-token option; every integration needs a Google identity.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any Verily host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verily-life-sciences/refs/heads/main/authentication/verily-life-sciences-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health
- Life Sciences
- Precision Health
- Clinical Research
- Biomedical Data
- FHIR
- Research Data Platform
- Trusted Research Environment
- Genomics
- Cloud Infrastructure
- Terraform
---
