---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Faunadb Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fauna declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fauna
provider_slug: faunadb-org
scheme_count: 1
schemes:
- evidence: Secrets are passed to the Fauna HTTP API as bearer tokens.
  header: Authorization
  location: header
  name: Fauna secret
  type: http-bearer
slug: faunadb-org-authentication
source_filename: faunadb-org-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.faunadb.org/fauna/current/learn/security/authentication/
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.faunadb.org/fauna/current/learn/security/authentication/\nsources:\n- https://docs.faunadb.org/fauna/current/learn/security/authentication/\n- https://docs.faunadb.org/fauna/current/build/tutorials/auth/\n- https://docs.faunadb.org/fauna/v4/build/tools/dashboard/mfa/\n- https://docs.faunadb.org/fauna/current/learn/security/tokens/\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Fauna secret\n  evidence: Secrets are passed to the Fauna HTTP API as bearer tokens.\n  location: header\n  header: Authorization\ndocs: https://docs.faunadb.org/fauna/current/learn/security/authentication/\n"
source_yaml_url: https://artifacts.apis.io/faunadb-org/authentication/faunadb-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Database
- Serverless
- NoSQL
- Cloud
---
