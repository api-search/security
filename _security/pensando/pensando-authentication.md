---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pensando Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pensando * declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pensando *
provider_slug: pensando
scheme_count: 2
schemes:
- detail: Configuration(psm_config_path=~/.psm/config.json, interactive_mode=True); credentials and PSM endpoint are read from the local config, or supplied interactively at runtime.
  mechanism: local config file
  type: appliance-credential
- detail: All PSM API traffic is HTTPS. verify_ssl is configurable in the client to accommodate self-signed appliance certificates.
  mechanism: https
  type: tls
slug: pensando-authentication
source_filename: pensando-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: github.com/pensando/pypi README + PSM Python SDK configuration module\napi: AMD Pensando Policy and Services Manager (PSM) REST API\ndocs: https://github.com/pensando/pypi/blob/main/README.md\nsummary: >-\n  The PSM REST API is authenticated per-appliance. The official Python bindings\n  authenticate via a local PSM credential/config file (~/.psm/config.json) that\n  carries the PSM endpoint and credentials; an interactive login mode is also\n  supported. TLS verification is configurable (verify_ssl) because PSM appliances\n  are commonly deployed with self-signed certificates. There is no public,\n  multi-tenant OAuth surface — auth is scoped to a customer's own PSM deployment.\nschemes:\n- type: appliance-credential\n  mechanism: local config file\n  detail: >-\n    Configuration(psm_config_path=~/.psm/config.json, interactive_mode=True);\n    credentials and PSM endpoint are read from the local config, or supplied\n    interactively\
  \ at runtime.\n- type: tls\n  mechanism: https\n  detail: >-\n    All PSM API traffic is HTTPS. verify_ssl is configurable in the client to\n    accommodate self-signed appliance certificates.\nnotes: >-\n  Auth details are documented via the SDK rather than a public hosted auth page;\n  the authoritative live docs are served from a running PSM instance at\n  https://<PSM-IP>/docs. No public OpenAPI/Swagger securitySchemes were available\n  to derive from, so no OAuth scopes artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pensando/refs/heads/main/authentication/pensando-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Enterprise
- Networking
- DPU
- Infrastructure
- Cloud
- Security
- AMD
---
