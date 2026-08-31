---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Shoreline cluster API, read from the only first-party documentation that is still published: the Shoreline Terraform provider docs in the archived source repository. Shoreline''s own docs host (docs.shoreline.io) no longer resolves, and there is no OpenAPI to derive securitySchemes from, so this profile is documentation-sourced rather than spec-derived.'
kind: authentication
layout: security
method: searched
name: Shoreline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shoreline declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Shoreline
provider_slug: shoreline
scheme_count: 1
schemes:
- credential_delivery:
    env_var: SHORELINE_TOKEN
    note: Provider docs state the token should be supplied via the SHORELINE_TOKEN environment variable, which is read during Configure and bypasses Terraform state and plan output; they explicitly warn against hardcoding it in a provider block or a .tfvars file.
    preferred: environment variable
  description: Customer/user-specific authorization token for the Shoreline API server. Documented as the provider's `token` argument, marked Sensitive.
  id: bearer_token
  in: header
  name: Authorization
  scheme: bearer
  type: http
slug: shoreline-authentication
source_filename: shoreline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Shoreline\nproviderId: shoreline\ngenerated: '2026-08-29'\nmodified: '2026-08-29'\nmethod: searched\nsource: https://github.com/NVIDIA/terraform-provider-shoreline/blob/main/docs/index.md\ndocs: https://registry.terraform.io/providers/shorelinesoftware/shoreline/latest/docs\ndescription: >-\n  Authentication profile for the Shoreline cluster API, read from the only first-party\n  documentation that is still published: the Shoreline Terraform provider docs in the archived\n  source repository. Shoreline's own docs host (docs.shoreline.io) no longer resolves, and there\n  is no OpenAPI to derive securitySchemes from, so this profile is documentation-sourced rather\n  than spec-derived.\napi_host:\n  form: customer-specific\n  template: '<CLUSTER_API_ENDPOINT>'\n  note: >-\n    There is no single public API host. The provider's `url` argument is documented as\n    \"Customer-specific URL for the\
  \ Shoreline API server\" — each customer's Shoreline cluster\n    exposes its own backend endpoint. This is why apis.yml carries no baseURL: the correct value\n    is templated per tenant, not omitted by oversight.\nschemes:\n  - id: bearer_token\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    description: >-\n      Customer/user-specific authorization token for the Shoreline API server. Documented as the\n      provider's `token` argument, marked Sensitive.\n    credential_delivery:\n      preferred: environment variable\n      env_var: SHORELINE_TOKEN\n      note: >-\n        Provider docs state the token should be supplied via the SHORELINE_TOKEN environment\n        variable, which is read during Configure and bypasses Terraform state and plan output;\n        they explicitly warn against hardcoding it in a provider block or a .tfvars file.\noauth2: false\nopenid_connect: false\nmutual_tls: unknown\napi_keys: false\nscopes:\n  published: false\n  note:\
  \ >-\n    No OAuth scope surface. The documented model is a single bearer token per customer/user, so\n    scopes/ is intentionally absent (the pipeline skips scopes/ for key- and token-auth providers).\nauthorization_model:\n  note: >-\n    The provider exposes a `shoreline_principal` resource (identity + name) and an\n    `allowed_entities` attribute on actions, notebooks and runbooks, indicating a\n    principal/entity-based authorization model on the backend. The reference for it was on\n    docs.shoreline.io and is no longer reachable, so no further detail is asserted here.\ncaveat: >-\n  Shoreline was acquired by NVIDIA in July 2024 and the source repository this documentation\n  lives in was archived in August 2026. Treat this profile as a historical record of a\n  decommissioned product, not as live integration guidance.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoreline/refs/heads/main/authentication/shoreline-authentication.yml
summary_line: 1 scheme
tags:
- AIOps
- Automation
- Incident Response
- Site Reliability Engineering
- Cloud Operations
- Remediation
- Observability
- Terraform
---
