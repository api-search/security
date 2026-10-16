---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for connecting Google or Microsoft 365 accounts uses OAuth 2.0 tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Caldavconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mediakreativ UG declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mediakreativ UG
provider_slug: caldavconnect
scheme_count: 1
schemes:
- evidence: Auf unserer Seite werden keine Passwörter gespeichert – der Zugriff erfolgt über ein widerrufbares OAuth-Token.
  flows:
  - authorization_code
  how_to_obtain: User clicks the connect button, is redirected to the provider (Google or Microsoft) to sign in and grant access, after which a revocable OAuth token is issued.
  name: Google/Microsoft OAuth
  type: oauth2
slug: caldavconnect-authentication
source_filename: caldavconnect-authentication.yml
source_heading: Authentication Profile
source_url: https://caldavconnect.de/de/docs/getting-started
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://caldavconnect.de/de/docs/getting-started\nsources:\n- https://caldavconnect.de/de/docs/getting-started\ndescription: Authentication for connecting Google or Microsoft 365 accounts uses OAuth 2.0 tokens.\nschemes:\n- type: oauth2\n  name: Google/Microsoft OAuth\n  evidence: Auf unserer Seite werden keine Passwörter gespeichert – der Zugriff erfolgt über ein widerrufbares OAuth-Token.\n  flows:\n  - authorization_code\n  how_to_obtain: User clicks the connect button, is redirected to the provider (Google or Microsoft) to sign in and grant access, after which\n    a revocable OAuth token is issued.\ndocs: https://caldavconnect.de/de/docs/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caldavconnect/refs/heads/main/authentication/caldavconnect-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CalDAV
- Sync
- Calendar
- GDPR
---
