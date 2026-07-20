---
api_key_in:
- header
api_specs:
- filename: leo-labs-platform-openapi.yml
  format: yaml
  label: LeoLabs Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/openapi/leo-labs-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Leo Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeoLabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LeoLabs
provider_slug: leo-labs
scheme_count: 1
schemes:
- credential_sources:
  - kind: environment
    variables:
    - LEOLABS_ACCESS_KEY
    - LEOLABS_SECRET_KEY
  - keys:
    - access_key
    - secret_key
    kind: file
    path: ~/.leolabs/config
    section: credentials
  - command: leolabs configure
    kind: cli
  description: 'LeoLabs access key / secret key pair, sent as `Authorization: basic <accessKey>:<secretKey>`.

    Despite the `basic` prefix this is not RFC 7617 HTTP Basic — the official LeoLabs client sends

    the two keys colon-joined and unencoded, with no base64 step. Keys are issued from the LeoLabs

    Platform (https://platform.leolabs.space/).

    '
  format: basic {accessKey}:{secretKey}
  in: header
  name: leolabsKeyPair
  parameter: Authorization
  sources:
  - openapi/leo-labs-platform-openapi.yml
  - https://pypi.org/project/leolabs/0.1.22/
  type: apiKey
slug: leo-labs-authentication
source_filename: leo-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/leo-labs-platform-openapi.yml\ndocs: https://docs.leolabs.space/\ndocs_note: LeoLabs' reference documentation at https://docs.leolabs.space/ is behind a\n  customer login (Document360), so the auth model below was derived from LeoLabs' own\n  published Python client (PyPI `leolabs` 0.1.22, `leolabs/cli/utils.py`) rather than\n  from the docs.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: Long-lived access key + secret key pair issued from the LeoLabs Platform.\n    There is no OAuth or token-exchange step on the v1 Platform API itself; the OAuth /\n    OIDC surface at auth.leolabs.space is the Okta org that fronts interactive login to\n    the LeoLabs Platform and documentation, not API authorization.\nschemes:\n- name: leolabsKeyPair\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'basic {accessKey}:{secretKey}'\n  description: |\n    LeoLabs access key / secret key pair,\
  \ sent as `Authorization: basic <accessKey>:<secretKey>`.\n    Despite the `basic` prefix this is not RFC 7617 HTTP Basic — the official LeoLabs client sends\n    the two keys colon-joined and unencoded, with no base64 step. Keys are issued from the LeoLabs\n    Platform (https://platform.leolabs.space/).\n  credential_sources:\n  - kind: environment\n    variables:\n    - LEOLABS_ACCESS_KEY\n    - LEOLABS_SECRET_KEY\n  - kind: file\n    path: ~/.leolabs/config\n    section: credentials\n    keys:\n    - access_key\n    - secret_key\n  - kind: cli\n    command: leolabs configure\n  sources:\n  - openapi/leo-labs-platform-openapi.yml\n  - https://pypi.org/project/leolabs/0.1.22/\ninteractive_login:\n  provider: Okta\n  issuer: https://auth.leolabs.space\n  discovery: https://auth.leolabs.space/.well-known/openid-configuration\n  applies_to: LeoLabs Platform and documentation sign-in (not the v1 Platform API key pair)\n  see: scopes/leo-labs-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/authentication/leo-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Space
- Satellites
- Space Situational Awareness
- Space Traffic Management
- Orbital Data
- Radar
- Aerospace
- Defense
- Geospatial
---
