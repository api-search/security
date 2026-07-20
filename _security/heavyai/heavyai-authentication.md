---
api_key_in: []
auth_types:
- username-password
- tls
description: ''
kind: authentication
layout: security
method: searched
name: Heavyai Authentication
name_suffix: Authentication
oauth_flows: []
overview: HEAVY.AI secures its APIs with username-password and tls across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HEAVY.AI
provider_slug: heavyai
scheme_count: 2
schemes:
- description: 'Clients (heavysql, the Python heavyai client, @heavyai/connector, JDBC/ODBC) authenticate to a HeavyDB server with a username and password against a named database (default database: heavyai). Connection parameters are user, password, host, port (default 6274), and database name.'
  name: username-password
  sources:
  - https://docs.nvidia.com/heavyai/apis-and-interfaces/heavysql
  type: credentials
- description: Connections can be encrypted by supplying a trusted server certificate (heavysql --ca-cert, or the equivalent client option), and the HTTP transport can be upgraded to HTTPS. TLS is optional and deployment-configured.
  name: tls
  sources:
  - https://docs.nvidia.com/heavyai/apis-and-interfaces/heavysql
  type: transport
slug: heavyai-authentication
source_filename: heavyai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.nvidia.com/heavyai/apis-and-interfaces\nnotes: >-\n  No OpenAPI/securitySchemes are published (HeavyDB exposes an Apache Thrift API,\n  native SQL, and JDBC/ODBC, not a REST/OpenAPI surface), so this profile is\n  grounded in the interface and heavysql documentation rather than derived from a\n  spec.\nsummary:\n  types:\n  - username-password\n  - tls\n  transport_encryption: optional-tls\n  oauth2_flows: []\nschemes:\n- name: username-password\n  type: credentials\n  description: >-\n    Clients (heavysql, the Python heavyai client, @heavyai/connector, JDBC/ODBC)\n    authenticate to a HeavyDB server with a username and password against a named\n    database (default database: heavyai). Connection parameters are user, password,\n    host, port (default 6274), and database name.\n  sources:\n  - https://docs.nvidia.com/heavyai/apis-and-interfaces/heavysql\n- name: tls\n  type: transport\n  description: >-\n  \
  \  Connections can be encrypted by supplying a trusted server certificate\n    (heavysql --ca-cert, or the equivalent client option), and the HTTP transport\n    can be upgraded to HTTPS. TLS is optional and deployment-configured.\n  sources:\n  - https://docs.nvidia.com/heavyai/apis-and-interfaces/heavysql\nenterprise_notes: >-\n  Heavy Immerse (the web application) additionally supports enterprise identity\n  integrations (LDAP / SAML / OAuth-based SSO) in the Enterprise Edition; verify\n  the exact mechanisms against the current security/administration docs before\n  relying on them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heavyai/refs/heads/main/authentication/heavyai-authentication.yml
summary_line: username-password/tls · 2 schemes
tags:
- Company
- Ai
- Analytics
- Database
- GPU
- SQL
- Geospatial
- Data Visualization
- Data Science
- Business Intelligence
---
