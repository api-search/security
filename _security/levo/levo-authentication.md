---
anonymous_access: false
api_key_in: []
auth_types: []
description: Levo uses a Satellite authorization key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Levo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Levo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Levo
provider_slug: levo
scheme_count: 1
schemes:
- evidence: The Levo-all package uses an authorization key to access Levo.ai.
  name: LEVOAI_AUTH_KEY
  type: apiKey
slug: levo-authentication
source_filename: levo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.levo.ai/quickstart
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.levo.ai/quickstart\nsources:\n- https://docs.levo.ai/quickstart\n- https://docs.levo.ai/quickstart/quickstart-mac\n- https://docs.levo.ai/quickstart/quickstart-kubernetes\n- https://docs.levo.ai/quickstart/quickstart-minikube\ndescription: Levo uses a Satellite authorization key for authentication.\nschemes:\n- type: apiKey\n  name: LEVOAI_AUTH_KEY\n  evidence: The Levo-all package uses an authorization key to access Levo.ai.\nnote: The documentation does not specify whether the key is sent in a header, query parameter, or body.\ndocs: https://docs.levo.ai/quickstart\n"
source_yaml_url: https://artifacts.apis.io/levo/authentication/levo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- AI
- API
- Platform
---
