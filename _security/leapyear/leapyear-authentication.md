---
api_key_in: []
auth_types:
- password
- public-key
description: ''
kind: authentication
layout: security
method: searched
name: Leapyear Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeapYear secures its APIs with password and public-key across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeapYear
provider_slug: leapyear
scheme_count: 3
schemes:
- description: Client(url=..., username=..., password=...) logs the user in through the default ly_login authenticate callback, which returns a LeapYear token held for the life of the connection.
  name: username-password
  parameters:
  - username
  - password
  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html
  type: password
- description: Client(..., public_key_auth=True) authenticates with public key credentials instead of a password. Credential problems surface as PublicKeyCredentialsError.
  name: public-key
  parameters:
  - public_key_auth
  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html
  type: public-key
- description: The authenticate parameter accepts a callback that performs the login and returns a LeapYear token, allowing a deployment to substitute its own identity flow.
  name: custom-authenticate-callback
  parameters:
  - authenticate
  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html
  type: pluggable
slug: leapyear-authentication
source_filename: leapyear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html\ndocs: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html\nnotes: >-\n  LeapYear published no OpenAPI, so this profile is taken from the first-party Python\n  client reference rather than derived from a spec. LeapYear Core is self-hosted: the\n  client authenticates against a customer-operated server, not a public multi-tenant\n  endpoint.\nsummary:\n  types:\n  - password\n  - public-key\n  api_key_in: []\n  oauth2_flows: []\n  token_model: server-issued session token\ndeployment:\n  model: self-hosted\n  default_url: http://localhost:4401\n  url_env_var: LY_API_URL\n  transport: https\n  note: >-\n    The Client url argument defaults to the LY_API_URL environment variable, falling\n    back to http://localhost:4401. Documented examples use port 4401 over TLS.\nschemes:\n- name: username-password\n  type: password\n \
  \ description: >-\n    Client(url=..., username=..., password=...) logs the user in through the default\n    ly_login authenticate callback, which returns a LeapYear token held for the life\n    of the connection.\n  parameters:\n  - username\n  - password\n  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html\n- name: public-key\n  type: public-key\n  description: >-\n    Client(..., public_key_auth=True) authenticates with public key credentials instead\n    of a password. Credential problems surface as PublicKeyCredentialsError.\n  parameters:\n  - public_key_auth\n  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html\n- name: custom-authenticate-callback\n  type: pluggable\n  description: >-\n    The authenticate parameter accepts a callback that performs the login and returns\n    a LeapYear token, allowing a deployment to substitute its own identity flow.\n  parameters:\n  - authenticate\n  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/leapyear.html\n\
  session:\n  connection_lifecycle: >-\n    Connections are opened explicitly and closed with Client.close(), or managed with\n    the Client context manager.\n  token_expiry_error: TokenExpiredError\nauthorization:\n  model: role and grant based\n  subjects:\n  - User\n  - Group\n  resources:\n  - Database\n  - Table\n  - View\n  controls:\n  - get_access / set_access with DatabaseAccessType\n  - leapyear.admin.grants permission grants\n  - Privacy Profile and privacy limit per database\n  source: https://leapyear-python-docs.readthedocs-hosted.com/en/4.1.1/api/admin.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapyear/refs/heads/main/authentication/leapyear-authentication.yml
summary_line: password/public-key · 3 schemes
tags:
- Company
- Data Privacy
- Differential Privacy
- Machine Learning
- Analytics
- Data Clean Rooms
- Privacy Enhancing Technologies
- Python
- Acquired
---
