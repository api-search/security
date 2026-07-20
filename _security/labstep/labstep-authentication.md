---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Labstep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Labstep secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Labstep
provider_slug: labstep
scheme_count: 2
schemes:
- description: Per-user API key generated from the Labstep application and sent on every request in an `apikey` request header. This is the documented and recommended authentication method.
  docs: https://help.labstep.com/en/articles/3636355
  in: header
  name: apikey
  parameter_name: apikey
  source: labstep/service/helpers.py getHeaders()
  type: apiKey
- description: Session/impersonation token passed as an Authorization Bearer credential. Used by the SDK's authenticateWithToken() and by tokens minted through the impersonate flow; not the primary documented developer path.
  name: bearer
  scheme: bearer
  source: labstep/entities/user/repository.py authenticateWithToken()
  type: http
slug: labstep-authentication
source_filename: labstep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://labsteppy.readthedocs.io/en/latest/source/installation_login.html ;\n  https://github.com/Labstep/labstepPy (labstep/service/helpers.py, labstep/entities/user/repository.py)\n  ; https://www.labstep.com/security\ndocs: https://help.labstep.com/en/articles/1786226-getting-started-with-the-labstep-api\nnote: Labstep publishes no OpenAPI definition, so this profile is captured from the\n  officially maintained Python SDK source and the published docs rather than derived\n  from securitySchemes.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  description: Per-user API key generated from the Labstep application and sent on\n    every request in an `apikey` request header. This is the documented and recommended\n    authentication method.\n  docs: https://help.labstep.com/en/articles/3636355\n\
  \  source: labstep/service/helpers.py getHeaders()\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Session/impersonation token passed as an Authorization Bearer credential.\n    Used by the SDK's authenticateWithToken() and by tokens minted through the impersonate\n    flow; not the primary documented developer path.\n  source: labstep/entities/user/repository.py authenticateWithToken()\ndeprecated:\n- name: password login\n  detail: Username/password login via POST /public-api/user/login is deprecated. The\n    SDK raises \"Login via password has been deprecated. Please use labstep.authenticate\n    with an API key instead.\"\n  source: labstep/entities/user/repository.py login()\naccount_level_controls:\n  sso:\n  - SAML\n  - Google SSO\n  mfa: true\n  ip_allowlisting: true\n  source: https://www.labstep.com/security\nexample: |\n  import labstep\n  user = labstep.authenticate('myaccount@labstep.com', 'MY_API_KEY')\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labstep/refs/heads/main/authentication/labstep-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Electronic Lab Notebook
- Life Sciences
- Laboratory
- Research Data Management
- Scientific Software
- Inventory Management
- Biotechnology
- Chemistry
- Compliance
---
