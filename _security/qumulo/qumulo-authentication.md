---
api_key_in: []
auth_types:
- http-bearer
- session
- saml
- oauth2-support-portal
description: Authentication profile for the Qumulo Core REST API, captured from the public REST API Guide (no OpenAPI is published, so this is documentation-sourced, not derived from a spec). Every Qumulo cluster serves its own API; clients authenticate to the cluster to receive a bearer credential.
kind: authentication
layout: security
method: searched
name: Qumulo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qumulo secures its APIs with http-bearer, session, saml, and oauth2-support-portal across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qumulo
provider_slug: qumulo
scheme_count: 3
schemes:
- docs: https://docs.qumulo.com/rest-api-guide/
  mechanism: POST credentials to session/login to obtain a session bearer token, which is then sent on subsequent requests. Primary programmatic auth for the qq CLI `login` command.
  name: SessionLogin
  type: session
- docs: https://docs.qumulo.com/rest-api-guide/
  mechanism: 'Long-lived bearer access tokens created and managed through the auth/access-tokens endpoints (qq auth_create_access_token / auth_modify_access_token). Sent as an Authorization: Bearer header.'
  name: AccessToken
  scheme: bearer
  type: http
- docs: https://docs.qumulo.com/rest-api-guide/
  mechanism: SAML-based single sign-on via session/start-saml-login and session/retrieve-saml-login (qq sso_login), for SSO-integrated clusters.
  name: SAML
  type: saml
slug: qumulo-authentication
source_filename: qumulo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qumulo.com/rest-api-guide/\ndocs: https://docs.qumulo.com/rest-api-guide/\ndescription: >-\n  Authentication profile for the Qumulo Core REST API, captured from the public\n  REST API Guide (no OpenAPI is published, so this is documentation-sourced, not\n  derived from a spec). Every Qumulo cluster serves its own API; clients\n  authenticate to the cluster to receive a bearer credential.\nsummary:\n  types: [http-bearer, session, saml, oauth2-support-portal]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: SessionLogin\n  type: session\n  mechanism: >-\n    POST credentials to session/login to obtain a session bearer token, which is\n    then sent on subsequent requests. Primary programmatic auth for the qq CLI\n    `login` command.\n  docs: https://docs.qumulo.com/rest-api-guide/\n- name: AccessToken\n  type: http\n  scheme: bearer\n  mechanism: >-\n    Long-lived bearer access tokens created and managed\
  \ through the\n    auth/access-tokens endpoints (qq auth_create_access_token /\n    auth_modify_access_token). Sent as an Authorization: Bearer header.\n  docs: https://docs.qumulo.com/rest-api-guide/\n- name: SAML\n  type: saml\n  mechanism: >-\n    SAML-based single sign-on via session/start-saml-login and\n    session/retrieve-saml-login (qq sso_login), for SSO-integrated clusters.\n  docs: https://docs.qumulo.com/rest-api-guide/\nnotes: >-\n  The care.qumulo.com support portal (separate from the cluster API) is a\n  Salesforce-backed property exposing its own OpenID Connect discovery document\n  (see well-known/qumulo-care-openid-configuration.json); it governs support\n  portal identity, not the Qumulo Core REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qumulo/refs/heads/main/authentication/qumulo-authentication.yml
summary_line: http-bearer/session/saml/oauth2-support-portal · 3 schemes
tags:
- Company
- Storage
- File Storage
- Data Platform
- Cloud Storage
- Unstructured Data
- Enterprise
- Infrastructure
- REST API
- CLI
---
