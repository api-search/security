---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kasten Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kasten secures its APIs with http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kasten
provider_slug: kasten
scheme_count: 5
schemes:
- description: 'Token authentication accepts any token the Kubernetes API server can verify (typically a ServiceAccount bearer token from `kubectl create token` or a service-account secret). Always enabled as a secondary auth type so the REST API can be called with an Authorization: Bearer <token> header. This is the primary mechanism for programmatic/API access.'
  name: TokenAuth
  scheme: bearer
  type: http
- description: htpasswd-generated username:password credentials supplied via Helm configuration at install time. Dashboard-oriented.
  name: BasicAuth
  scheme: basic
  type: http
- description: Integrates with an external OpenID Connect provider; extracts the user's ID from the token and uses Kubernetes User Impersonation so user-initiated actions are attributed to the authenticated identity.
  name: OIDC
  type: openIdConnect
- description: Native integration with the OpenShift OAuth server for clusters running on OpenShift.
  name: OpenShiftOAuth
  type: oauth2
- description: Authentication through a corporate Active Directory / LDAP directory service.
  name: LDAP
  scheme: ldap
  type: http
slug: kasten-authentication
source_filename: kasten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.kasten.io/latest/access/authentication.html\ndocs: https://docs.kasten.io/latest/access/authentication.html\nnote: >-\n  Veeam Kasten (Kasten K10) has no public OpenAPI spec to derive from; it is a\n  self-hosted, Kubernetes-native product whose dashboard and REST API sit behind\n  the K10 gateway in-cluster. Authentication is delegated to Kubernetes. This\n  profile is captured from the documented authentication options.\nsummary:\n  types: [http, oauth2, openIdConnect]\n  api_key_in: []\n  primary_api_auth: bearer-token (Kubernetes ServiceAccount)\nschemes:\n  - name: TokenAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Token authentication accepts any token the Kubernetes API server can verify\n      (typically a ServiceAccount bearer token from `kubectl create token` or a\n      service-account secret). Always enabled as a secondary auth type so the REST\n      API can be called with an\
  \ Authorization: Bearer <token> header. This is the\n      primary mechanism for programmatic/API access.\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      htpasswd-generated username:password credentials supplied via Helm\n      configuration at install time. Dashboard-oriented.\n  - name: OIDC\n    type: openIdConnect\n    description: >-\n      Integrates with an external OpenID Connect provider; extracts the user's ID\n      from the token and uses Kubernetes User Impersonation so user-initiated\n      actions are attributed to the authenticated identity.\n  - name: OpenShiftOAuth\n    type: oauth2\n    description: >-\n      Native integration with the OpenShift OAuth server for clusters running on\n      OpenShift.\n  - name: LDAP\n    type: http\n    scheme: ldap\n    description: >-\n      Authentication through a corporate Active Directory / LDAP directory\n      service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kasten/refs/heads/main/authentication/kasten-authentication.yml
summary_line: http/oauth2/openIdConnect · 5 schemes
tags:
- Company
- Cybersecurity
- Kubernetes
- Backup
- Disaster Recovery
- Data Protection
- Cloud Native
- DevOps
---
