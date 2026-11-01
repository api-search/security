---
anonymous_access: false
api_key_in: []
api_specs:
- filename: phoebe-ai-openapi-generated.yml
  format: yaml
  label: Phoebe API
  slug: phoebe-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phoebe-ai/openapi/_ae-authored/phoebe-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Coral
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Phoebe Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phoebe declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Phoebe
provider_slug: phoebe-ai
scheme_count: 1
schemes:
- authorize_url: https://auth.<coral-host>
  evidence: 'Make sure you have an OIDC compatible identity provider: Self-hosted Coral requires that you have your own IdP that Coral can use to authenticate users.'
  flows:
  - authorization_code
  how_to_obtain: Configure an application on your IdP and provide the client_id and client_secret in the Coral configuration (see CORAL_OIDC_CLIENT_SECRET).
  name: OIDC
  type: oauth2
slug: phoebe-ai-authentication
source_filename: phoebe-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://withcoral.com/docs/getting-started/install-locally
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://withcoral.com/docs/getting-started/install-locally\nsources:\n- https://withcoral.com/docs/getting-started/install-locally\n- https://withcoral.com/docs/getting-started/quickstart\n- https://withcoral.com/docs/getting-started/self-host\n- https://withcoral.com/docs/getting-started/self-host/kubernetes\ndescription: Authentication schemes for Coral\nschemes:\n- type: oauth2\n  name: OIDC\n  evidence: 'Make sure you have an OIDC compatible identity provider: Self-hosted Coral requires that you have your own IdP that Coral can use\n    to authenticate users.'\n  flows:\n  - authorization_code\n  authorize_url: https://auth.<coral-host>\n  how_to_obtain: Configure an application on your IdP and provide the client_id and client_secret in the Coral configuration (see CORAL_OIDC_CLIENT_SECRET).\ndocs: https://withcoral.com/docs/getting-started/install-locally\n"
source_yaml_url: https://artifacts.apis.io/phoebe-ai/authentication/phoebe-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Machine-Learning
- Platform
- Ethics
- Enterprise
---
