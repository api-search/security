---
api_key_in: []
auth_types:
- application-privilege
- code-signing
description: ''
kind: authentication
layout: security
method: searched
name: Axiado Corporation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axiado Corporation secures its APIs with application-privilege and code-signing across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Axiado Corporation
provider_slug: axiado-corporation
scheme_count: 3
schemes:
- description: Secure applications execute either in privileged mode (direct hardware and register access, used for device drivers and system services) or in a sandboxed non-privileged mode that still reaches all TCU features. Axiado recommends non-privileged mode. Certain ADK APIs require the calling application to have been provisioned with special access privileges; the per-API access restrictions and the provisioning procedure are documented in the ADK API manual.
  name: application-privilege
  scope: firmware application
  source: https://devhub.axiado.com/docs/getting-started-with-securestack-adk
  type: authorization
- algorithms:
  - ECC
  - RSA
  description: All firmware images are signed as part of the build environment. The developer hub documents signed image creation with ECC or RSA keys, a signature-verification engine, root key management and a key store as first-class ADK engines. AX_STATUS_KEY_REJECTED, AX_STATUS_NO_KEY, AX_STATUS_KEY_EXP and AX_STATUS_VERSION_REVOKED are the published failure codes on this path.
  name: firmware-image-signing
  references:
  - https://devhub.axiado.com/reference/digital-signature-verification
  - https://devhub.axiado.com/reference/root-key-management
  - https://devhub.axiado.com/reference/key-store
  - https://devhub.axiado.com/reference/x509-certificate-management
  scope: TCU firmware image
  type: code-signing
- description: The TCU integrates a hardware root of trust, TPM and HSM on-die; the trusted execution environment anchoring ADK applications is rooted in that silicon rather than in a credential presented per request.
  name: hardware-root-of-trust
  scope: silicon
  source: https://axiado.com/tcu-platform/
  type: platform
slug: axiado-corporation-authentication
source_filename: axiado-corporation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://devhub.axiado.com/docs/getting-started-with-securestack-adk\napi: Axiado SecureStack ADK\ndocs: https://devhub.axiado.com/docs/getting-started-with-securestack-adk\nnote: >-\n  Derived mechanically first — 0-working/derive-authentication.py found no OpenAPI\n  securitySchemes to read, because Axiado publishes no OpenAPI. This profile is therefore\n  searched from the developer hub. The ADK is an embedded API: there are no API keys, bearer\n  tokens, OAuth flows or mutual-TLS schemes. Authorization is a firmware application-privilege\n  model plus cryptographic image signing.\nsummary:\n  types: [application-privilege, code-signing]\n  api_key_in: []\n  oauth2_flows: []\n  http_schemes: []\n  bearer: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: application-privilege\n  type: authorization\n  scope: firmware application\n  description: >-\n    Secure applications execute either\
  \ in privileged mode (direct hardware and register access,\n    used for device drivers and system services) or in a sandboxed non-privileged mode that\n    still reaches all TCU features. Axiado recommends non-privileged mode. Certain ADK APIs\n    require the calling application to have been provisioned with special access privileges;\n    the per-API access restrictions and the provisioning procedure are documented in the ADK\n    API manual.\n  source: https://devhub.axiado.com/docs/getting-started-with-securestack-adk\n- name: firmware-image-signing\n  type: code-signing\n  scope: TCU firmware image\n  description: >-\n    All firmware images are signed as part of the build environment. The developer hub\n    documents signed image creation with ECC or RSA keys, a signature-verification engine,\n    root key management and a key store as first-class ADK engines. AX_STATUS_KEY_REJECTED,\n    AX_STATUS_NO_KEY, AX_STATUS_KEY_EXP and AX_STATUS_VERSION_REVOKED are the published\n    failure\
  \ codes on this path.\n  algorithms: [ECC, RSA]\n  references:\n  - https://devhub.axiado.com/reference/digital-signature-verification\n  - https://devhub.axiado.com/reference/root-key-management\n  - https://devhub.axiado.com/reference/key-store\n  - https://devhub.axiado.com/reference/x509-certificate-management\n- name: hardware-root-of-trust\n  type: platform\n  scope: silicon\n  description: >-\n    The TCU integrates a hardware root of trust, TPM and HSM on-die; the trusted execution\n    environment anchoring ADK applications is rooted in that silicon rather than in a\n    credential presented per request.\n  source: https://axiado.com/tcu-platform/\nportal_access:\n  developer_hub_login: https://devhub.axiado.com/login\n  note: >-\n    The developer hub itself has an account login, and ADK sources are released by Axiado\n    customer engineering on request — access to the SDK is commercial, not self-serve.\nnot_applicable:\n  api_keys: no hosted API to key\n  oauth2: no authorization\
  \ server; /.well-known/oauth-authorization-server returns 404\n  openid_connect: /.well-known/openid-configuration returns 404 on both hosts\n  scopes: no OAuth surface — scopes/ artifact deliberately not created\nx-evidence:\n  fetched: '2026-07-31'\n  derive_script: 0-working/derive-authentication.py (0 auth profiles — no OpenAPI in repo)\n  probes:\n  - {url: 'https://devhub.axiado.com/.well-known/oauth-authorization-server', http_status: 404}\n  - {url: 'https://axiado.com/.well-known/openid-configuration', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiado-corporation/refs/heads/main/authentication/axiado-corporation-authentication.yml
summary_line: application-privilege/code-signing · 3 schemes
tags:
- Semiconductors
- Hardware Security
- Platform Security
- Data-Center
- Cybersecurity
- Baseboard Management Controller
- Root of Trust
- Firmware
- Embedded
- Cryptography
- AI Infrastructure
- Trusted Computing
- OpenBMC
- SDK
---
