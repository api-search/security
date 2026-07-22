---
api_key_in:
- file
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Valtix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valtix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Valtix
provider_slug: valtix
scheme_count: 1
schemes:
- description: API key issued per Valtix tenant and downloaded as a JSON key file; used by the Terraform provider (api_key_file argument) to authenticate against the Valtix Controller.
  name: controller-api-key
  sources:
  - https://registry.terraform.io/providers/valtix-security/valtix/latest/docs
  type: apiKey
slug: valtix-authentication
source_filename: valtix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.valtix.com/userguide/administration/roles/\ndocs: https://docs.valtix.com/userguide/\nnotes: >-\n  Valtix publishes no OpenAPI; the supported programmatic interface is the\n  verified Terraform provider (valtix-security/valtix), which authenticates to\n  the Valtix Controller with a tenant API key file generated in the Valtix\n  Portal. Portal/console access supports SSO (SAML via Okta, Azure AD,\n  OneLogin), MFA, and mutual TLS, with three tenant roles.\nsummary:\n  types: [apiKey]\n  api_key_in: [file]\n  oauth2_flows: []\nschemes:\n  - name: controller-api-key\n    type: apiKey\n    description: >-\n      API key issued per Valtix tenant and downloaded as a JSON key file; used\n      by the Terraform provider (api_key_file argument) to authenticate against\n      the Valtix Controller.\n    sources:\n      - https://registry.terraform.io/providers/valtix-security/valtix/latest/docs\nconsole:\n  sso:\n    -\
  \ saml (Okta)\n    - saml (Azure AD)\n    - saml (OneLogin)\n    - azure-ad-non-saml\n  mfa: true\n  mutual_tls: documented (userguide/administration/users/mtl/)\nroles:\n  - id: admin_super\n    name: Super Admin\n    permissions: Modify (all settings)\n  - id: admin_rw\n    name: Read/Write Admin\n    permissions: Modify (except Super Admin management)\n  - id: admin_read-only\n    name: Read-Only Admin\n    permissions: Read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valtix/refs/heads/main/authentication/valtix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Cloud Security
- Network Security
- Multicloud
- Firewall
- Terraform
---
