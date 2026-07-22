---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Virtualmin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Virtualmin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Virtualmin
provider_slug: virtualmin
scheme_count: 1
schemes:
- description: HTTP Basic authentication as the Webmin master administrator against https://<host>:10000/virtual-server/remote.cgi. Sent as standard Authorization headers (e.g. wget --http-user / --http-passwd, or LWP credentials against the "Webmin Server" realm).
  name: basicAuth
  scheme: basic
  sources:
  - docs/development/remote-api
  type: http
slug: virtualmin-authentication
source_filename: virtualmin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.virtualmin.com/docs/development/remote-api/\ndocs: https://www.virtualmin.com/docs/development/remote-api/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  oauth2_flows: []\n  api_key_in: []\n  note: >-\n    The Remote API authenticates over HTTP Basic against Webmin's own user database,\n    the same credentials as the web interface. It is accessible only to the master\n    administrator (typically the Unix `root` account) for security reasons; there is\n    no OAuth, API-key or token scheme. The command-line API instead relies on local\n    Unix root/system access. No OAuth scopes exist, so no scopes/ artifact is produced.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication as the Webmin master administrator against\n    https://<host>:10000/virtual-server/remote.cgi. Sent as standard Authorization\n    headers (e.g. wget --http-user / --http-passwd,\
  \ or LWP credentials against the\n    \"Webmin Server\" realm).\n  sources: [docs/development/remote-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtualmin/refs/heads/main/authentication/virtualmin-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web Hosting
- Control Panel
- Server Management
- Webmin
- DNS
- Email
- Domains
- Virtual Servers
- Databases
- SSL
- WordPress
- Open Source
- Linux
---
