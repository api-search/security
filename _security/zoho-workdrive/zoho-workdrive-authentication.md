---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Zoho Docs as published on the developer pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zoho Workdrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zoho Docs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zoho Docs
provider_slug: zoho-workdrive
scheme_count: 2
schemes:
- evidence: Zoho's OAuth implementation uses Bearer authentication scheme , hence while making API calls, the access token has to be passed in the Authorization header with the prefix Bearer .
  header: Authorization
  how_to_obtain: Register the app in the Zoho API console to get a Client ID and Client Secret, then use either the authorization code grant flow (generate an authorization code and exchange it for an access token and refresh token) or the client credentials grant flow (provide client credentials to obtain an access token). The access token is sent in the Authorization header as "Bearer <access-token>".
  location: header
  name: OAuth 2.0
  type: oauth2
- evidence: If you want your app to fetch data from your own Zoho account, or set up app-to-app communication in the backend without any user interaction, you can use the Self Client option.
  header: Authorization
  how_to_obtain: Create a Self Client in the Zoho API console to obtain a Client ID and Client Secret. Then obtain an access token either via the authorization code grant flow (generate an authorization code in the console and exchange it) or via the client credentials grant flow (send client credentials to receive an access token). The token is used as a Bearer token in the Authorization header.
  location: header
  name: OAuth 2.0 (Self Client)
  type: oauth2
slug: zoho-workdrive-authentication
source_filename: zoho-workdrive-authentication.yml
source_heading: Authentication Profile
source_url: https://www.zoho.com/developer/oauth/self-client/overview.html
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.zoho.com/developer/oauth/self-client/overview.html\nsources:\n- https://www.zoho.com/developer/oauth/self-client/overview.html\n- https://www.zoho.com/developer/oauth/introduction.html\n- https://www.zoho.com/developer/oauth/multi-dc-support.html\n- https://www.zoho.com/developer/oauth/incremental-authorization/overview.html\ndescription: Authentication methods for Zoho Docs as published on the developer pages.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Zoho's OAuth implementation uses Bearer authentication scheme , hence while making API calls, the access token has to be passed in\n    the Authorization header with the prefix Bearer .\n  location: header\n  header: Authorization\n  how_to_obtain: Register the app in the Zoho API console to get a Client ID and Client Secret, then use either the authorization code grant flow\n    (generate an authorization\
  \ code and exchange it for an access token and refresh token) or the client credentials grant flow (provide client\n    credentials to obtain an access token). The access token is sent in the Authorization header as \"Bearer <access-token>\".\n- type: oauth2\n  name: OAuth 2.0 (Self Client)\n  evidence: If you want your app to fetch data from your own Zoho account, or set up app-to-app communication in the backend without any user\n    interaction, you can use the Self Client option.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Self Client in the Zoho API console to obtain a Client ID and Client Secret. Then obtain an access token either via\n    the authorization code grant flow (generate an authorization code in the console and exchange it) or via the client credentials grant flow\n    (send client credentials to receive an access token). The token is used as a Bearer token in the Authorization header.\ndocs: https://www.zoho.com/developer/oauth/self-client/overview.html\n"
source_yaml_url: https://artifacts.apis.io/zoho-workdrive/authentication/zoho-workdrive-authentication.yml
summary_line: 2 schemes
tags:
- Cloud Storage
- Collaboration
- File Management
- Zoho
- SaaS
---
