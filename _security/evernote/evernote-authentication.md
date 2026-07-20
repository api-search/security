---
api_key_in: []
auth_types:
- oauth1
- developer-token
description: ''
kind: authentication
layout: security
method: searched
name: Evernote Authentication
name_suffix: Authentication
oauth_flows: []
overview: evernote secures its APIs with oauth1 and developer-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: evernote
provider_slug: evernote
scheme_count: 2
schemes:
- authorize_url: https://www.evernote.com/OAuth.action
  credentials:
  - consumer key (API key)
  - consumer secret
  description: Three-legged OAuth 1.0a. Request a temporary token, redirect the user to authorize, then exchange the verifier for a long-lived access token. Access tokens do not expire unless revoked by the user. Recommended for public applications, webhooks, and advanced permissions.
  legs: 3
  name: OAuth 1.0a
  sandbox_base: https://sandbox.evernote.com
  temporary_credential_url: https://www.evernote.com/oauth
  token_url: https://www.evernote.com/oauth
  type: oauth1
- description: A long-lived personal token that grants instant API access to the developer's own account without the OAuth handshake. Intended for single-user scripts and prototyping, not for accessing other users' accounts.
  issue_url: https://dev.evernote.com/doc/articles/dev_tokens.php
  name: Developer Token
  type: developer-token
slug: evernote-authentication
source_filename: evernote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.evernote.com/doc/articles/authentication.php\ndocs: https://dev.evernote.com/doc/articles/authentication.php\nsummary:\n  types: [oauth1, developer-token]\n  oauth_version: '1.0a'\n  scopes: false\n  note: >-\n    The Evernote Cloud API (EDAM) is not OpenAPI/OAuth2-based; it is a Thrift\n    service. Authentication produces an authenticationToken that is passed as a\n    parameter to every UserStore/NoteStore call.\nschemes:\n- name: OAuth 1.0a\n  type: oauth1\n  legs: 3\n  temporary_credential_url: https://www.evernote.com/oauth\n  authorize_url: https://www.evernote.com/OAuth.action\n  token_url: https://www.evernote.com/oauth\n  sandbox_base: https://sandbox.evernote.com\n  description: >-\n    Three-legged OAuth 1.0a. Request a temporary token, redirect the user to\n    authorize, then exchange the verifier for a long-lived access token. Access\n    tokens do not expire unless revoked by the user. Recommended\
  \ for public\n    applications, webhooks, and advanced permissions.\n  credentials:\n  - consumer key (API key)\n  - consumer secret\n- name: Developer Token\n  type: developer-token\n  issue_url: https://dev.evernote.com/doc/articles/dev_tokens.php\n  description: >-\n    A long-lived personal token that grants instant API access to the developer's\n    own account without the OAuth handshake. Intended for single-user scripts and\n    prototyping, not for accessing other users' accounts.\npermissions:\n  note: >-\n    Evernote uses per-application permission levels (e.g. read-only vs full\n    access) negotiated when an API key is activated, rather than OAuth scopes.\n  docs: https://dev.evernote.com/doc/articles/permissions.php\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evernote/refs/heads/main/authentication/evernote-authentication.yml
summary_line: oauth1/developer-token · 2 schemes
tags:
- Company
- Note Taking
- Productivity
- Knowledge Management
- Notes
- Content
- SaaS
- Sync
---
