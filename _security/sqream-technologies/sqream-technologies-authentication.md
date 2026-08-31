---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sqream Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: SQream Technologies declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SQream Technologies
provider_slug: sqream-technologies
scheme_count: 2
schemes:
- description: A SQreamDB role name and its password, supplied on connect via --username/--password (CLI) or the equivalent driver connection parameters. Passwords are prompted interactively when omitted.
  id: role-password
  location: connection handshake
  parameters:
  - username
  - password
  source: https://docs.sqream.com/en/latest/reference/cli/sqream_sql.html
  type: basic-credentials
- description: LDAP authentication against Microsoft Active Directory or another directory service. Only roles with admin privileges or higher may enable it; once enabled, authorization for all existing and newly added roles is handled by the LDAP server, with the exception of the initial deployment `sqream` role which retains full control permissions.
  id: ldap
  source: https://docs.sqream.com/en/latest/configuration_guides/ldap.html
  type: directory
slug: sqream-technologies-authentication
source_filename: sqream-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.sqream.com/en/latest/operational_guides/access_control.html\ndocs:\n- https://docs.sqream.com/en/latest/operational_guides/access_control.html\n- https://docs.sqream.com/en/latest/configuration_guides/ldap.html\n- https://docs.sqream.com/en/latest/reference/cli/sqream_sql.html\nnote: >-\n  SQream has no HTTP API and therefore no HTTP security schemes — there is no apiKey header, no\n  bearer token, no OAuth 2.0 flow and no OpenID Connect discovery document (every\n  /.well-known/openid-configuration and /.well-known/oauth-authorization-server probe 404s; see\n  well-known/sqream-technologies-well-known.yml). Authentication happens at the database connection:\n  a role name and password are presented over SQream's wire protocol by the client driver or CLI, and\n  authorization is role-based access control in the database itself. Because there is no OAuth\n  surface, no scopes/ artifact is emitted — the permission\
  \ model is SQL GRANT/REVOKE, not scopes.\ntransport: SQream wire protocol over TCP (default port 5000 standalone, 3108 via the load balancer)\nschemes:\n- id: role-password\n  type: basic-credentials\n  location: connection handshake\n  parameters:\n  - username\n  - password\n  description: >-\n    A SQreamDB role name and its password, supplied on connect via --username/--password (CLI) or the\n    equivalent driver connection parameters. Passwords are prompted interactively when omitted.\n  source: https://docs.sqream.com/en/latest/reference/cli/sqream_sql.html\n- id: ldap\n  type: directory\n  description: >-\n    LDAP authentication against Microsoft Active Directory or another directory service. Only roles\n    with admin privileges or higher may enable it; once enabled, authorization for all existing and\n    newly added roles is handled by the LDAP server, with the exception of the initial deployment\n    `sqream` role which retains full control permissions.\n  source: https://docs.sqream.com/en/latest/configuration_guides/ldap.html\n\
  authorization:\n  model: RBAC (role-based access control)\n  description: >-\n    SQreamDB manages authentication and authorization with role-based access control in the manner of\n    ANSI SQL. Permissions are of two kinds — global permissions, held by SUPERUSER roles, granting\n    unrestricted access to all system and database activity; and object-level permissions, assignable\n    to non-SUPERUSER roles over databases, schemas, tables, functions, views, foreign tables, catalogs\n    and services.\n  source: https://docs.sqream.com/en/latest/operational_guides/access_control.html\ntransport_security:\n  tls: optional\n  description: >-\n    Traffic in and out of SQreamDB can be encrypted with TLS, configured manually on the connector\n    (ODBC, JDBC and the SQL client's --ssl flag). TLS is not on by default — the CLI's --ssl flag\n    defaults to false.\n  source: https://docs.sqream.com/en/latest/reference/cli/sqream_sql.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sqream-technologies/refs/heads/main/authentication/sqream-technologies-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Database
- Data Warehouse
- Analytics
- GPU
- SQL
- Big Data
- Machine Learning
- Data Ingestion
- Israel
---
