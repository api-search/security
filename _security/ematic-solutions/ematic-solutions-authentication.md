---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ematic Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ematic Solutions declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ematic Solutions
provider_slug: ematic-solutions
scheme_count: 1
schemes:
- format: ematic-apikey=<ematic-key>,esp-apikey=<esp-key>
  id: ematic-esp-composite-key
  in: header
  name: Authorization
  note: This is a non-standard composite key header, not RFC 7235 Basic/Bearer. A client that sends only one of the two keys receives HTTP 401 with body {"message":"missing apikeys"}; a wrong key returns {"message":"invalid apikeys"}.
  parts:
  - description: Ematic API key generated when the client account is created. Published format is "<hash>-<suffix>", where the suffix identifies the data center (for example "sg1").
    doubles_as: host-routing
    key: ematic-apikey
  - description: API key of the connected Email Service Provider account.
    key: esp-apikey
  required: true
  type: apiKey
slug: ematic-solutions-authentication
source_filename: ematic-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://kb.ematicsolutions.com/restful-api/developer-guide.html\ndocs: https://kb.ematicsolutions.com/restful-api/developer-guide.html\napi: Ematic Solutions Core API\nsummary: >-\n  The Core API authenticates with a single HTTP Authorization header that carries TWO keys at once —\n  the Ematic API key issued for the client account, and the API key of the connected ESP (Email\n  Service Provider). Both are required on every request; there is no OAuth, no OpenID Connect and no\n  bearer-token flow. The Ematic API key doubles as the routing key: its suffix names the data center\n  the account lives in and therefore the host the request must be sent to.\nschemes:\n- id: ematic-esp-composite-key\n  type: apiKey\n  in: header\n  name: Authorization\n  format: 'ematic-apikey=<ematic-key>,esp-apikey=<esp-key>'\n  required: true\n  parts:\n  - key: ematic-apikey\n    description: >-\n      Ematic API key generated when the client account\
  \ is created. Published format is\n      \"<hash>-<suffix>\", where the suffix identifies the data center (for example \"sg1\").\n    doubles_as: host-routing\n  - key: esp-apikey\n    description: API key of the connected Email Service Provider account.\n  note: >-\n    This is a non-standard composite key header, not RFC 7235 Basic/Bearer. A client that sends only\n    one of the two keys receives HTTP 401 with body {\"message\":\"missing apikeys\"}; a wrong key\n    returns {\"message\":\"invalid apikeys\"}.\noauth: false\noidc: false\nmtls: false\nscopes: none\nkey_management:\n  issuance: >-\n    Issued by Ematic at client-account creation. There is no self-service developer signup or key\n    rotation surface documented in the public knowledge base.\n  rotation: undocumented\n  prefixes:\n  - pattern: '<hash>-<suffix>'\n    example_suffix: sg1\n    meaning: suffix names the data center / host shard\nplatform_roles:\n  source: https://kb.ematicsolutions.com/new-to-ematic/access-rights.html\n\
  \  note: >-\n    The Ematic platform UI has its own role model (Admin, Email Performance report, Billing, Hi-iQ,\n    Bye-iQ, Retry-iQ) governing human access to platform.ematicsolutions.com. These roles are NOT\n    API scopes and do not constrain Core API keys.\n  roles: [Admin, Email Performance report, Billing, Hi-iQ, Bye-iQ, Retry-iQ]\ngaps:\n- No OAuth 2.0 / OIDC surface; no /.well-known/oauth-authorization-server (probed 404 on every host).\n- No documented key rotation, expiry or revocation procedure.\n- Credentials are placed in a custom-formatted Authorization header rather than a standard scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ematic-solutions/refs/heads/main/authentication/ematic-solutions-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketing
- Digital Marketing
- Marketing Technology
- MarTech
- Email Marketing
- CRM
- E-Commerce
- Analytics
- Consulting
- Asia Pacific
---
