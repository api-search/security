---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xplenty-openapi-generated.yml
  format: yaml
  label: Integrate.io API
  slug: xplenty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xplenty/openapi/_ae-authored/xplenty-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Integrate.io as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Xplenty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Integrate.io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Integrate.io
provider_slug: xplenty
scheme_count: 3
schemes:
- authorize_url: https://accounts.google.com/o/oauth2/v2/auth
  evidence: Universal OAuth is a flexible authentication service that allows you to connect to any OAuth-based API.
  how_to_obtain: Enter your Client ID, Client Secret, and the provider’s OAuth URLs, then click 'Authenticate' to open a popup where you log in and authorize the app. The connection is then established.
  name: Universal OAuth (Authorization Code Flow)
  type: oauth2
- evidence: You can use HubSpot Private Apps to connect your HubSpot account securely with Integrate.io using an Access Token (Bearer Token).
  header: Authorization
  how_to_obtain: Create a HubSpot Private App, copy the generated Access Token, and paste it into the Integrate.io connection configuration.
  location: header
  name: HubSpot Access Token (Private App)
  type: http-bearer
- evidence: Authorization string header required Enter your API key as the username. Leave the password field blank.
  header: Authorization
  how_to_obtain: 'Use your Integrate.io API key as the username in a Basic Authorization header (e.g., "Authorization: Basic <encoded-value>").'
  location: header
  name: Integrate.io API Key Basic Auth
  type: http-basic
slug: xplenty-authentication
source_filename: xplenty-authentication.yml
source_heading: Authentication Profile
source_url: https://www.integrate.io/docs/etl/allowing-integrateio-etl-access-to-any-api-with-oauth
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.integrate.io/docs/etl/allowing-integrateio-etl-access-to-any-api-with-oauth\nsources:\n- https://www.integrate.io/docs/etl/allowing-integrateio-etl-access-to-any-api-with-oauth\n- https://www.integrate.io/docs/etl/2-factor-authentication\n- https://www.integrate.io/docs/etl/allowing-integrateio-etl-access-to-hubspot-service-token\n- https://www.integrate.io/docs/api-reference/users/regenerate-authenticated-user-tokens\ndescription: Authentication methods supported by Integrate.io as documented.\nschemes:\n- type: oauth2\n  name: Universal OAuth (Authorization Code Flow)\n  evidence: Universal OAuth is a flexible authentication service that allows you to connect to any OAuth-based API.\n  authorize_url: https://accounts.google.com/o/oauth2/v2/auth\n  how_to_obtain: Enter your Client ID, Client Secret, and the provider’s OAuth URLs, then click 'Authenticate' to open a\
  \ popup where you log in\n    and authorize the app. The connection is then established.\n- type: http-bearer\n  name: HubSpot Access Token (Private App)\n  evidence: You can use HubSpot Private Apps to connect your HubSpot account securely with Integrate.io using an Access Token (Bearer Token).\n  location: header\n  header: Authorization\n  how_to_obtain: Create a HubSpot Private App, copy the generated Access Token, and paste it into the Integrate.io connection configuration.\n- type: http-basic\n  name: Integrate.io API Key Basic Auth\n  evidence: Authorization string header required Enter your API key as the username. Leave the password field blank.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Use your Integrate.io API key as the username in a Basic Authorization header (e.g., \"Authorization: Basic <encoded-value>\").'\ndocs: https://www.integrate.io/docs/etl/allowing-integrateio-etl-access-to-any-api-with-oauth\nnote: 2 extracted row(s) were dropped because their\
  \ quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/xplenty/authentication/xplenty-authentication.yml
summary_line: 3 schemes
tags:
- Data Integration
- ETL
- Low-Code
- Artificial Intelligence
- Cloud
---
