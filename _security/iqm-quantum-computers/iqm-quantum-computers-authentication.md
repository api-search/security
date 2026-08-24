---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Iqm Quantum Computers Authentication
name_suffix: Authentication
oauth_flows: []
overview: IQM Quantum Computers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IQM Quantum Computers
provider_slug: iqm-quantum-computers
scheme_count: 1
schemes:
- credential_delivery:
  - mechanism: environment variable
    name: IQM_TOKEN
  - mechanism: constructor parameter
    name: token
    true: IQMProvider / IQMClient
  - mechanism: tokens file
    name: IQM_TOKENS_FILE
    note: Path to a tokens file; legacy Cortex CLI flow
  description: A long-lived, non-recoverable IQM Resonance API token generated once from the Resonance web dashboard ("Generate token"). It is sent on every request as an Authorization header. Regenerating the token immediately invalidates the previous one; IQM warns the value cannot be retrieved again after the dialog is closed.
  in: header
  name: IQMToken
  parameter_name: Authorization
  provisioning:
    docs: https://docs.iqm.tech/iqm-client/user_guide_qiskit.html#authentication
    self_service: true
    steps:
    - Sign in to the IQM Resonance dashboard
    - Select "Generate token" on the Dashboard page
    - Copy the token before closing the window (it is not recoverable)
    surface: https://resonance.iqm.tech
  scheme: bearer
  sources:
  - https://pypi.org/project/iqm-client/
  - https://docs.iqm.tech/iqm-client/user_guide_qiskit.html
  type: http
slug: iqm-quantum-computers-authentication
source_filename: iqm-quantum-computers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: openapi/ (none published)\ndocs: https://docs.iqm.tech/iqm-client/user_guide_qiskit.html#authentication\nnote: >-\n  DERIVED FROM FIRST-PARTY SOURCE, NOT FROM AN OPENAPI. IQM publishes no OpenAPI/Swagger\n  document, so this profile is reconstructed from two public first-party sources: the\n  authentication section of IQM's own Qiskit-on-IQM user guide, and the Apache-2.0\n  `iqm-client` 35.0.1 source distribution on PyPI\n  (src/iqm/iqm_server_client/iqm_server_client.py). It is NOT a transcription of a provider\n  securityScheme block, and it is not represented as one.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: IQMToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  description: >-\n    A long-lived, non-recoverable IQM Resonance API token generated once\
  \ from the Resonance\n    web dashboard (\"Generate token\"). It is sent on every request as an Authorization\n    header. Regenerating the token immediately invalidates the previous one; IQM warns the\n    value cannot be retrieved again after the dialog is closed.\n  provisioning:\n    surface: https://resonance.iqm.tech\n    steps:\n    - Sign in to the IQM Resonance dashboard\n    - Select \"Generate token\" on the Dashboard page\n    - Copy the token before closing the window (it is not recoverable)\n    self_service: true\n    docs: https://docs.iqm.tech/iqm-client/user_guide_qiskit.html#authentication\n  credential_delivery:\n  - {mechanism: environment variable, name: IQM_TOKEN}\n  - {mechanism: constructor parameter, name: token, on: IQMProvider / IQMClient}\n  - {mechanism: tokens file, name: IQM_TOKENS_FILE, note: \"Path to a tokens file; legacy Cortex CLI flow\"}\n  sources: [https://pypi.org/project/iqm-client/, https://docs.iqm.tech/iqm-client/user_guide_qiskit.html]\ntransport_security:\n\
  \  https_required: true\n  note: >-\n    iqm-client 35.0.0 made this enforceable client-side: the client raises on plain-HTTP\n    requests to remote hosts, strips the Authorization header if an insecure remote call is\n    attempted anyway, and blocks automatic redirects for mutating requests. Recorded because\n    it is an unusually explicit credential-leak defence for a client library.\n  evidence: https://docs.iqm.tech/iqm-client/changelog.html\ngated_surfaces:\n- url: https://resonance.iqm.tech/\n  status: 401\n  note: Every unauthenticated path returns {\"error_code\":\"unauthorized\",\"request_id\":...,\"message\":...}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iqm-quantum-computers/refs/heads/main/authentication/iqm-quantum-computers-authentication.yml
summary_line: http · 1 scheme
tags:
- Quantum Computing
- Quantum Cloud
- High Performance Computing
- Research
- Scientific Computing
- Developer Tools
- Protobuf
- Hardware
- Finland
- Deep Tech
---
