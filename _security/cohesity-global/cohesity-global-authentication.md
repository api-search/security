---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Cohesity Global Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cohesity Global secures its APIs with apiKey, http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cohesity Global
provider_slug: cohesity-global
scheme_count: 4
schemes:
- applies_to: Helios (multi-cluster SaaS control plane)
  in: header
  name: HeliosApiKey
  parameter: apiKey
  source: https://github.com/cohesity/cohesity_sdk
  type: apiKey
- applies_to: Helios (multi-cluster SaaS control plane)
  authorizationUrl: https://helios.cohesity.com/oauth2/authorize
  flow: authorizationCode
  name: HeliosOAuth2
  scopes:
  - openid
  - email
  - profile
  - cohesity_user
  - cohesity_viewer
  - cohesity_gaia_viewer
  source: https://helios.cohesity.com/.well-known/openid-configuration
  tokenUrl: https://helios.cohesity.com/oauth2/token
  type: oauth2
- applies_to: Helios (multi-cluster SaaS control plane)
  name: HeliosOIDC
  openIdConnectUrl: https://helios.cohesity.com/.well-known/openid-configuration
  source: https://helios.cohesity.com/.well-known/openid-configuration
  type: openIdConnect
- applies_to: On-premises Cohesity cluster (VIP + username/password + domain, exchanged for a session token)
  name: ClusterCredentials
  scheme: basic
  source: https://github.com/cohesity/cohesity_sdk
  type: http
slug: cohesity-global-authentication
source_filename: cohesity-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.cohesity.com/ and https://github.com/cohesity/cohesity_sdk\ndocs: https://developer.cohesity.com/docs/get-started-apps.html\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  notes: Cohesity Helios uses an API key presented in the request header for programmatic access, and\n    also runs a full OAuth2/OIDC authorization-code (PKCE S256) flow discoverable at\n    https://helios.cohesity.com/.well-known/openid-configuration. On-premises Cohesity clusters\n    authenticate with username/password (plus AD/LDAP domain) to obtain a session token used on\n    subsequent calls.\nschemes:\n- name: HeliosApiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  applies_to: Helios (multi-cluster SaaS control plane)\n  source: https://github.com/cohesity/cohesity_sdk\n- name: HeliosOAuth2\n  type: oauth2\n  flow: authorizationCode\n\
  \  authorizationUrl: https://helios.cohesity.com/oauth2/authorize\n  tokenUrl: https://helios.cohesity.com/oauth2/token\n  scopes: [openid, email, profile, cohesity_user, cohesity_viewer, cohesity_gaia_viewer]\n  applies_to: Helios (multi-cluster SaaS control plane)\n  source: https://helios.cohesity.com/.well-known/openid-configuration\n- name: HeliosOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://helios.cohesity.com/.well-known/openid-configuration\n  applies_to: Helios (multi-cluster SaaS control plane)\n  source: https://helios.cohesity.com/.well-known/openid-configuration\n- name: ClusterCredentials\n  type: http\n  scheme: basic\n  applies_to: On-premises Cohesity cluster (VIP + username/password + domain, exchanged for a session token)\n  source: https://github.com/cohesity/cohesity_sdk\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohesity-global/refs/heads/main/authentication/cohesity-global-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Data Security
- Data Management
- Backup and Recovery
- Cyber Resilience
- Data Protection
- Disaster Recovery
- Cloud
---
