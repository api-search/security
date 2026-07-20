---
api_key_in: []
auth_types:
- fix-session
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Electronx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electronx secures its APIs with fix-session and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Electronx
provider_slug: electronx
scheme_count: 2
schemes:
- description: Each FIX session authenticates with a unique SenderCompID assigned by ElectronX during provisioning, combined with SSL/TLS encryption. The Logon (35=A) message carries the FIX version, heartbeat interval (30s), and target (EXI). SenderSubID (Tag 50) must NOT be sent in Logon (rejects the session) but IS required on all order-related messages for audit trail.
  name: fix-sendercompid
  sources:
  - https://docs.electronx.com/fix-guide
  type: fix-session
- description: All FIX sessions (Order Entry, Market Data, Drop Copy) run over SSL/TLS. Firm-specific gateway hostnames and ports are delivered privately in a FIX Connectivity Details document during provisioning, not published publicly.
  name: ssl-tls
  sources:
  - https://docs.electronx.com/fix-guide
  type: mutualTLS
slug: electronx-authentication
source_filename: electronx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.electronx.com/fix-guide\nnote: >-\n  ElectronX exposes no HTTP/REST API and publishes no OpenAPI, so this profile is\n  captured from the FIX API guide rather than derived from securitySchemes. Access\n  is via FIX sessions authenticated by a provisioned SenderCompID over SSL/TLS.\nsummary:\n  types:\n  - fix-session\n  - mutualTLS\n  transport: FIXT.1.1 (session) + FIX 5.0 SP2 (application)\nschemes:\n- name: fix-sendercompid\n  type: fix-session\n  description: >-\n    Each FIX session authenticates with a unique SenderCompID assigned by\n    ElectronX during provisioning, combined with SSL/TLS encryption. The Logon\n    (35=A) message carries the FIX version, heartbeat interval (30s), and target\n    (EXI). SenderSubID (Tag 50) must NOT be sent in Logon (rejects the session)\n    but IS required on all order-related messages for audit trail.\n  sources:\n  - https://docs.electronx.com/fix-guide\n- name: ssl-tls\n\
  \  type: mutualTLS\n  description: >-\n    All FIX sessions (Order Entry, Market Data, Drop Copy) run over SSL/TLS.\n    Firm-specific gateway hostnames and ports are delivered privately in a FIX\n    Connectivity Details document during provisioning, not published publicly.\n  sources:\n  - https://docs.electronx.com/fix-guide\nsendercompid_conventions:\n- session: Order Entry\n  format: D-{TRADING_DESK_ID}-OE{nn}\n  example: D-POLARIS-01-OE01\n- session: Market Data\n  format: '{CUSTOMER_LABEL}-MD{nn}'\n  example: POLARIS-MD01\n- session: Drop Copy\n  format: CM-{CLEARING_MEMBER_ID}-DC{nn}\n  example: CM-POLARIS-DC01\nplatform_access:\n  docs: https://docs.electronx.com/platform-access\n  note: >-\n    GUI platform access uses first-login credentials with multi-factor\n    authentication (MFA). API (FIX) access is provisioned separately.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electronx/refs/heads/main/authentication/electronx-authentication.yml
summary_line: fix-session/mutualTLS · 2 schemes
tags:
- Company
- Energy
- Electricity
- Power Derivatives
- Trading
- Exchange
- Financial Services
- FIX API
- Market Data
- Futures
- Options
- CFTC
---
