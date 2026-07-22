---
api_key_in: []
auth_types:
- http
- mauth
description: ''
kind: authentication
layout: security
method: searched
name: Medidata Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medidata Solutions secures its APIs with http and mauth across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Medidata Solutions
provider_slug: medidata-solutions
scheme_count: 2
schemes:
- description: The external calling system supplies a Rave username and password using HTTP Basic authentication over HTTPS. Simplest to set up but subject to password expiry, so Medidata recommends MAuth for long-lived integrations.
  name: HTTP Basic
  scheme: basic
  sources:
  - docs
  type: http
- clients:
  - https://github.com/mdsol/requests-mauth
  - https://github.com/mdsol/mauth-client-python
  description: 'Medidata''s MAuth (Mutual Authentication) request-signing scheme. The client signs each request with an RSA private key tied to an MAuth App ID; the server verifies against the registered public key. A user account associated with an MAuth App ID does not have password expiry, making MAuth the preferred approach for long-term integrations. Client libraries: requests-mauth (Python/requests) and mauth-client.'
  name: MAuth
  scheme: request-signing
  sources:
  - https://techblog.mdsol.com/2015/12/08/rwslib-and-mauth.html
  type: http
slug: medidata-solutions-authentication
source_filename: medidata-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://techblog.mdsol.com/2015/12/08/rwslib-and-mauth.html\ndocs: https://rwslib.readthedocs.io/en/latest/getting_started.html\nsummary:\n  types: [http, mauth]\n  http_schemes: [basic]\n  note: >-\n    Rave Web Services has no published OpenAPI; auth model captured from the\n    RWS documentation, the Medidata tech blog, and the rwslib client library.\nschemes:\n- name: HTTP Basic\n  type: http\n  scheme: basic\n  description: >-\n    The external calling system supplies a Rave username and password using\n    HTTP Basic authentication over HTTPS. Simplest to set up but subject to\n    password expiry, so Medidata recommends MAuth for long-lived integrations.\n  sources: [docs]\n- name: MAuth\n  type: http\n  scheme: request-signing\n  description: >-\n    Medidata's MAuth (Mutual Authentication) request-signing scheme. The client\n    signs each request with an RSA private key tied to an MAuth App ID; the\n    server verifies\
  \ against the registered public key. A user account associated\n    with an MAuth App ID does not have password expiry, making MAuth the\n    preferred approach for long-term integrations. Client libraries:\n    requests-mauth (Python/requests) and mauth-client.\n  clients:\n  - https://github.com/mdsol/requests-mauth\n  - https://github.com/mdsol/mauth-client-python\n  sources: [https://techblog.mdsol.com/2015/12/08/rwslib-and-mauth.html]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata-solutions/refs/heads/main/authentication/medidata-solutions-authentication.yml
summary_line: http/mauth · 2 schemes
tags:
- Company
- Healthcare
- Clinical Trials
- Life Sciences
- Electronic Data Capture
- EDC
- Pharma
- CDISC ODM
- Clinical Data Management
- Dassault Systemes
---
