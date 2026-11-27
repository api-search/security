---
anonymous_access: false
api_key_in: []
auth_types: []
description: OpenWater uses OAuth 2.0 for SSO connectors.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Openwater Authentication
name_suffix: Authentication
oauth_flows: []
overview: Openwater declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Openwater
provider_slug: openwater
scheme_count: 1
schemes:
- authorize_url: Login Url (Auth Url)
  evidence: 'In return your IT admin should give you the following: 1. Login Url (Auth Url) 2. Client ID 3. Client Secret 4. Token Url Endpoint 5. User Info / Profile Url Endpoint 6. Scope(s).'
  how_to_obtain: Provide the Login URL (Auth Url), Client ID, Client Secret, Token URL Endpoint, User Info/Profile URL, and Scopes from the identity provider to the OpenWater Integrations Hub connector.
  name: Basic OAuth
  type: oauth2
slug: openwater-authentication
source_filename: openwater-authentication.yml
source_heading: Authentication Profile
source_url: https://help.getopenwater.com/en/articles/6473347-connect-an-sso-with-an-identity-provider-using-oauth-and-integrations-hub.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.getopenwater.com/en/articles/6473347-connect-an-sso-with-an-identity-provider-using-oauth-and-integrations-hub.md\nsources:\n- https://help.getopenwater.com/en/articles/6473347-connect-an-sso-with-an-identity-provider-using-oauth-and-integrations-hub.md\n- https://help.getopenwater.com/en/articles/7067497-connect-an-sso-with-imis-ems-using-oauth-and-integrations-hub.md\n- https://help.getopenwater.com/en/articles/7022376-connect-an-sso-with-yourmembership-using-oauth-and-integrations-hub.md\n- https://help.getopenwater.com/en/articles/7035479-connect-an-sso-with-memberclicks-using-oauth-and-integrations-hub.md\ndescription: OpenWater uses OAuth 2.0 for SSO connectors.\nschemes:\n- type: oauth2\n  name: Basic OAuth\n  evidence: 'In return your IT admin should give you the following: 1. Login Url (Auth Url) 2. Client ID 3. Client Secret 4. Token Url Endpoint\n    5. User\
  \ Info / Profile Url Endpoint 6. Scope(s).'\n  authorize_url: Login Url (Auth Url)\n  how_to_obtain: Provide the Login URL (Auth Url), Client ID, Client Secret, Token URL Endpoint, User Info/Profile URL, and Scopes from the identity\n    provider to the OpenWater Integrations Hub connector.\nnote: The page does not list explicit URLs, token endpoint values, or scope strings; they are to be supplied by the identity provider.\ndocs: https://help.getopenwater.com/en/articles/6473347-connect-an-sso-with-an-identity-provider-using-oauth-and-integrations-hub.md\n"
source_yaml_url: https://artifacts.apis.io/openwater/authentication/openwater-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software-as-a-Service
- Application Management
- Grants
- Education
---
