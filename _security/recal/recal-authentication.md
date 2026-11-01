---
anonymous_access: false
api_key_in: []
api_specs:
- filename: recal-organization-api-openapi.yml
  format: yaml
  label: Recal Organization API
  slug: recal-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-api-openapi.yml
- filename: recal-organization-scheduling-api-openapi.yml
  format: yaml
  label: Recal Organization Scheduling API
  slug: recal-organization-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-scheduling-api-openapi.yml
- filename: recal-organizations-calendar-api-openapi.yml
  format: yaml
  label: Recal Organizations Calendar API
  slug: recal-organizations-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organizations-calendar-api-openapi.yml
- filename: recal-user-calendar-api-openapi.yml
  format: yaml
  label: Recal User Calendar API
  slug: recal-user-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-calendar-api-openapi.yml
- filename: recal-user-oauth-api-openapi.yml
  format: yaml
  label: Recal User OAuth API
  slug: recal-user-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-oauth-api-openapi.yml
- filename: recal-user-scheduling-api-openapi.yml
  format: yaml
  label: Recal User Scheduling API
  slug: recal-user-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-scheduling-api-openapi.yml
- filename: recal-users-api-openapi.yml
  format: yaml
  label: Recal Users API
  slug: recal-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-users-api-openapi.yml
auth_types: []
description: Recal uses OAuth2 Authorization Code flow to connect to Google Calendar and Microsoft Outlook Calendar. Clients must register an OAuth app with the provider, configure the redirect URL to https://dash.recal.dev/oauth/<provider>, and add the client ID, client secret, and redirect URL in the Recal dashboard.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Recal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Recal
provider_slug: recal
scheme_count: 1
schemes:
- evidence: Before you paste Each prompt uses the dashboard's hosted callback, https://dash.recal.dev/oauth/<provider> . That address works for connecting calendars from the dashboard; if you run your own callback, replace it — in the prompt and in Recal — before you start.
  flows:
  - authorization_code
  how_to_obtain: Register an application in Azure, obtain the Client ID and Client Secret, and add them along with the redirect URL to Recal.
  name: Microsoft OAuth
  scopes:
  - User.Read
  - Calendars.ReadWrite
  - Calendars.ReadWrite.Shared
  - Calendars.Read
  type: oauth2
slug: recal-authentication
source_filename: recal-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.recal.dev/core/oauth/google
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.recal.dev/core/oauth/google\nsources:\n- https://docs.recal.dev/core/oauth/google\n- https://docs.recal.dev/core/oauth\n- https://docs.recal.dev/core/oauth/microsoft\n- https://docs.recal.dev/core/oauth/setup-prompt\ndescription: Recal uses OAuth2 Authorization Code flow to connect to Google Calendar and Microsoft Outlook Calendar. Clients must register an\n  OAuth app with the provider, configure the redirect URL to https://dash.recal.dev/oauth/<provider>, and add the client ID, client secret, and\n  redirect URL in the Recal dashboard.\nschemes:\n- type: oauth2\n  name: Microsoft OAuth\n  evidence: Before you paste Each prompt uses the dashboard's hosted callback, https://dash.recal.dev/oauth/<provider> . That address works for\n    connecting calendars from the dashboard; if you run your own callback, replace it — in the prompt and in Recal — before you start.\n\
  \  flows:\n  - authorization_code\n  scopes:\n  - User.Read\n  - Calendars.ReadWrite\n  - Calendars.ReadWrite.Shared\n  - Calendars.Read\n  how_to_obtain: Register an application in Azure, obtain the Client ID and Client Secret, and add them along with the redirect URL to Recal.\ndocs: https://docs.recal.dev/core/oauth/google\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/recal/authentication/recal-authentication.yml
summary_line: 1 scheme
tags:
- Calendar API
- Scheduling
- SDK
- Multi-Tenant
- Recruiting
- Marketplace
- AI Agents
---
