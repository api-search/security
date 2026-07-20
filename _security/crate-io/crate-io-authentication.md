---
api_key_in:
- header
auth_types:
- http-basic
- http-basic-apikey
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Crate Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crate Io secures its APIs with http-basic, http-basic-apikey, and jwt across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crate Io
provider_slug: crate-io
scheme_count: 3
schemes:
- applies_to: CrateDB Cloud API (https://console.cratedb.cloud/api/v2)
  description: HTTP Basic authentication using a CrateDB Cloud API key id (username) and secret (password). Keys are generated from the account settings page and inherit the permissions of the user who created them.
  docs: https://cratedb.com/docs/cloud/en/latest/reference/api.html
  name: cloud-api-key
  scheme: basic
  type: http
- applies_to: CrateDB HTTP SQL endpoint / PostgreSQL wire protocol
  description: CrateDB database users authenticate with username/password (HTTP Basic on the /_sql endpoint, or standard PostgreSQL auth on the wire protocol), governed by host-based access control (HBA) rules.
  docs: https://cratedb.com/docs/crate/reference/en/latest/admin/auth/index.html
  name: db-user-password
  scheme: basic
  type: http
- applies_to: CrateDB HTTP SQL endpoint
  bearerFormat: JWT
  description: CrateDB supports JWT-based authentication for database users, configurable through HBA rules (jwt auth method).
  docs: https://cratedb.com/docs/crate/reference/en/latest/admin/auth/methods.html
  name: db-jwt
  scheme: bearer
  type: http
slug: crate-io-authentication
source_filename: crate-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://cratedb.com/docs/cloud/en/latest/reference/api.html + https://cratedb.com/docs\nsummary:\n  types: [http-basic, http-basic-apikey, jwt]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: cloud-api-key\n  type: http\n  scheme: basic\n  applies_to: CrateDB Cloud API (https://console.cratedb.cloud/api/v2)\n  description: >-\n    HTTP Basic authentication using a CrateDB Cloud API key id (username) and\n    secret (password). Keys are generated from the account settings page and\n    inherit the permissions of the user who created them.\n  docs: https://cratedb.com/docs/cloud/en/latest/reference/api.html\n- name: db-user-password\n  type: http\n  scheme: basic\n  applies_to: CrateDB HTTP SQL endpoint / PostgreSQL wire protocol\n  description: >-\n    CrateDB database users authenticate with username/password (HTTP Basic on\n    the /_sql endpoint, or standard PostgreSQL auth on the wire protocol),\n    governed\
  \ by host-based access control (HBA) rules.\n  docs: https://cratedb.com/docs/crate/reference/en/latest/admin/auth/index.html\n- name: db-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: CrateDB HTTP SQL endpoint\n  description: >-\n    CrateDB supports JWT-based authentication for database users, configurable\n    through HBA rules (jwt auth method).\n  docs: https://cratedb.com/docs/crate/reference/en/latest/admin/auth/methods.html\ntransport_security:\n  tls: required-in-cloud\n  note: CrateDB Cloud endpoints are TLS-only; self-managed clusters can enable SSL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crate-io/refs/heads/main/authentication/crate-io-authentication.yml
summary_line: http-basic/http-basic-apikey/jwt · 3 schemes
tags:
- Company
- Database
- SQL
- Distributed Database
- Analytics
- Time Series
- Vector Database
- IoT
- Cloud
- Developer Tools
---
