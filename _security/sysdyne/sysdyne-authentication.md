---
api_key_in:
- credential-exchange
auth_types:
- session
- publicKeyExchange
description: ''
kind: authentication
layout: security
method: searched
name: Sysdyne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sysdyne Technologies secures its APIs with session and publicKeyExchange across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sysdyne Technologies
provider_slug: sysdyne
scheme_count: 2
schemes:
- description: RSA public key retrieved via the GetPublicKey operation, used to encrypt AppID/AppKey and user credentials before login.
  name: WebcretePublicKeyExchange
  operation: GetPublicKey
  sources:
  - wsdl/sysdyne-webcrete.wsdl
  type: publicKey
- description: Session established via Login / Login2 using the AppID/AppKey issued by Sysdyne; the resulting session context authorizes ProcessRequest calls and is torn down by Logout.
  name: WebcreteSessionLogin
  operations:
  - Login
  - Login2
  - Logout
  sources:
  - wsdl/sysdyne-webcrete.wsdl
  type: session
slug: sysdyne-authentication
source_filename: sysdyne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://api1.concretego.com/webcreteapi.asmx?WSDL +\n  https://github.com/sysdynetechnologies/WebcreteAPIExplorer\nnotes: >-\n  The ConcreteGO \"Webcrete\" API is a SOAP web service that does not declare its\n  security in an OpenAPI document, so the auth profile below is reconstructed\n  from the published WSDL operations and the official example clients rather than\n  derived mechanically. Authentication is a public-key credential exchange\n  followed by a session login: the client fetches an RSA public key\n  (GetPublicKey), encrypts its AppID/AppKey + user credentials, calls Login /\n  Login2 to obtain a session, and then submits work through ProcessRequest until\n  Logout. Producer-issued AppID / AppKey is a prerequisite for access.\nsummary:\n  types: [session, publicKeyExchange]\n  transport: SOAP (basicHttpBinding, SOAP 1.1 + 1.2)\n  api_key_in: [credential-exchange]\n  oauth2_flows: []\nschemes:\n  - name: WebcretePublicKeyExchange\n\
  \    type: publicKey\n    description: >-\n      RSA public key retrieved via the GetPublicKey operation, used to encrypt\n      AppID/AppKey and user credentials before login.\n    operation: GetPublicKey\n    sources: [wsdl/sysdyne-webcrete.wsdl]\n  - name: WebcreteSessionLogin\n    type: session\n    description: >-\n      Session established via Login / Login2 using the AppID/AppKey issued by\n      Sysdyne; the resulting session context authorizes ProcessRequest calls and\n      is torn down by Logout.\n    operations: [Login, Login2, Logout]\n    sources: [wsdl/sysdyne-webcrete.wsdl]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysdyne/refs/heads/main/authentication/sysdyne-authentication.yml
summary_line: session/publicKeyExchange · 2 schemes
tags:
- Company
- Concrete
- Construction
- Ready-Mix
- Dispatch
- Logistics
- ERP Integration
- SOAP
- Fleet Telematics
---
