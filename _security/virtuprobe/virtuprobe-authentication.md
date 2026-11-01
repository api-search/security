---
anonymous_access: false
api_key_in: []
api_specs:
- filename: virtuprobe-openapi-generated.yml
  format: yaml
  label: VirtuProbe Studio API
  slug: virtuprobe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/virtuprobe/openapi/_ae-authored/virtuprobe-openapi-generated.yml
auth_types: []
description: Authentication schemes supported by VirtuProbe Studio as documented.
kind: authentication
layout: security
mechanism_count: 10
method: searched
name: Virtuprobe Authentication
name_suffix: Authentication
oauth_flows: []
overview: VirtuProbe Studio declares 10 security scheme(s) across its OpenAPI definitions.
provider_name: VirtuProbe Studio
provider_slug: virtuprobe
scheme_count: 10
schemes:
- evidence: 'Basic Username + password ( Authorization: Basic )'
  header: Authorization
  location: header
  name: Basic
  type: http-basic
- evidence: Bearer Static bearer token
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: API Key Named key sent as a header, query parameter, or cookie
  location: header/query/cookie
  name: API Key
  type: apiKey
- evidence: Digest RFC 7616 challenge-response
  header: Authorization
  location: header
  name: Digest
  type: http-digest
- evidence: OAuth2 Client Credentials, Password, Authorization Code and Device Code grants.
  flows:
  - client_credentials
  - password
  - authorization_code
  - device_code
  header: Authorization
  location: header
  name: OAuth2
  type: oauth2
- evidence: NTLM Windows challenge-response with username + password
  header: Authorization
  location: header
  name: NTLM
  type: http-ntlm
- evidence: Pass-the-Hash (PTH) NTLM using a 32-character hex NT hash, no cleartext password
  header: Authorization
  location: header
  name: Pass-the-Hash (PTH)
  type: other
- evidence: 'SPNEGO / Kerberos Authorization: Negotiate ticket obtained from a KDC for HTTP/<host>'
  header: Authorization
  location: header
  name: SPNEGO / Kerberos
  type: other
- evidence: AWS SigV4 AWS request signing
  location: header
  name: AWS SigV4
  type: other
- evidence: Scripted A JavaScript script computes the auth headers at send time
  location: header
  name: Scripted
  type: other
slug: virtuprobe-authentication
source_filename: virtuprobe-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.virtuprobe.studio/credentials/overview/
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.virtuprobe.studio/credentials/overview/\nsources:\n- https://docs.virtuprobe.studio/credentials/overview/\n- https://docs.virtuprobe.studio/agents/api-access/\n- https://docs.virtuprobe.studio/getting-started/introduction/\n- https://docs.virtuprobe.studio/getting-started/installation/\ndescription: Authentication schemes supported by VirtuProbe Studio as documented.\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: 'Basic Username + password ( Authorization: Basic )'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Bearer\n  evidence: Bearer Static bearer token\n  location: header\n  header: Authorization\n- type: apiKey\n  name: API Key\n  evidence: API Key Named key sent as a header, query parameter, or cookie\n  location: header/query/cookie\n- type: http-digest\n  name: Digest\n  evidence: Digest RFC 7616 challenge-response\n \
  \ location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth2\n  evidence: OAuth2 Client Credentials, Password, Authorization Code and Device Code grants.\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  - password\n  - authorization_code\n  - device_code\n- type: http-ntlm\n  name: NTLM\n  evidence: NTLM Windows challenge-response with username + password\n  location: header\n  header: Authorization\n- type: other\n  name: Pass-the-Hash (PTH)\n  evidence: Pass-the-Hash (PTH) NTLM using a 32-character hex NT hash, no cleartext password\n  location: header\n  header: Authorization\n- type: other\n  name: SPNEGO / Kerberos\n  evidence: 'SPNEGO / Kerberos Authorization: Negotiate ticket obtained from a KDC for HTTP/<host>'\n  location: header\n  header: Authorization\n- type: other\n  name: AWS SigV4\n  evidence: AWS SigV4 AWS request signing\n  location: header\n- type: other\n  name: Scripted\n  evidence: Scripted A JavaScript script computes\
  \ the auth headers at send time\n  location: header\nnote: OAuth2 token and authorize URLs, as well as specific scopes, are not listed on the pages; they are left null/empty.\ndocs: https://docs.virtuprobe.studio/credentials/overview/\n"
source_yaml_url: https://artifacts.apis.io/virtuprobe/authentication/virtuprobe-authentication.yml
summary_line: 10 schemes
tags:
- Company
- Monitoring
- API Observability
- Analytics
- Alerts
---
