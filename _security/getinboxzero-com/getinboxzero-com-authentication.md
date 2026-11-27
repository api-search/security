---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getinboxzero-com-rules-api-openapi.yml
  format: yaml
  label: Inbox Zero Rules API
  slug: getinboxzero-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-rules-api-openapi.yml
- filename: getinboxzero-com-senders-api-openapi.yml
  format: yaml
  label: Inbox Zero Senders API
  slug: getinboxzero-com-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-senders-api-openapi.yml
- filename: getinboxzero-com-stats-api-openapi.yml
  format: yaml
  label: Inbox Zero Stats API
  slug: getinboxzero-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-stats-api-openapi.yml
auth_types: []
description: Authentication methods for Inbox Zero API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Inbox Zero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inbox Zero declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Inbox Zero
provider_slug: getinboxzero-com
scheme_count: 2
schemes:
- evidence: Configure Google OAuth credentials, scopes, and required APIs
  flows:
  - authorization_code
  how_to_obtain: Create OAuth credentials in Google Cloud Console, then copy the Client ID and secret into the .env file as GOOGLE_CLIENT_ID and GOOGLE_CLIENT_SECRET.
  name: Google OAuth
  scopes:
  - https://www.googleapis.com/auth/userinfo.profile
  - https://www.googleapis.com/auth/userinfo.email
  - https://www.googleapis.com/auth/gmail.modify
  - https://www.googleapis.com/auth/gmail.settings.basic
  - https://www.googleapis.com/auth/contacts
  - https://www.googleapis.com/auth/calendar.readonly
  - https://www.googleapis.com/auth/calendar.events
  - https://www.googleapis.com/auth/calendar.freebusy
  - https://www.googleapis.com/auth/drive.file
  - https://www.googleapis.com/auth/drive
  type: oauth2
- evidence: Configure Azure app registration and Microsoft Graph permissions
  flows:
  - authorization_code
  how_to_obtain: Register an app in Microsoft Azure Portal, then copy the Application (client) ID, Directory (tenant) ID (if single‑tenant), and client secret into the .env file as MICROSOFT_CLIENT_ID, MICROSOFT_TENANT_ID, and MICROSOFT_CLIENT_SECRET.
  name: Microsoft OAuth
  scopes:
  - openid
  - profile
  - email
  - User.Read
  - offline_access
  - Mail.ReadWrite
  - Mail.Send
  - MailboxSettings.ReadWrite
  - Calendars.Read
  - Calendars.ReadWrite
  - Files.ReadWrite
  - Contacts.Read
  - People.Read
  type: oauth2
slug: getinboxzero-com-authentication
source_filename: getinboxzero-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getinboxzero.com/essentials/api-keys.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getinboxzero.com/essentials/api-keys.md\nsources:\n- https://docs.getinboxzero.com/essentials/api-keys.md\n- https://docs.getinboxzero.com/hosting/google-oauth.md\n- https://docs.getinboxzero.com/hosting/microsoft-oauth.md\n- https://docs.getinboxzero.com/essentials/getting-started.md\ndescription: Authentication methods for Inbox Zero API\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: Configure Google OAuth credentials, scopes, and required APIs\n  flows:\n  - authorization_code\n  scopes:\n  - https://www.googleapis.com/auth/userinfo.profile\n  - https://www.googleapis.com/auth/userinfo.email\n  - https://www.googleapis.com/auth/gmail.modify\n  - https://www.googleapis.com/auth/gmail.settings.basic\n  - https://www.googleapis.com/auth/contacts\n  - https://www.googleapis.com/auth/calendar.readonly\n  - https://www.googleapis.com/auth/calendar.events\n\
  \  - https://www.googleapis.com/auth/calendar.freebusy\n  - https://www.googleapis.com/auth/drive.file\n  - https://www.googleapis.com/auth/drive\n  how_to_obtain: Create OAuth credentials in Google Cloud Console, then copy the Client ID and secret into the .env file as GOOGLE_CLIENT_ID and\n    GOOGLE_CLIENT_SECRET.\n- type: oauth2\n  name: Microsoft OAuth\n  evidence: Configure Azure app registration and Microsoft Graph permissions\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - profile\n  - email\n  - User.Read\n  - offline_access\n  - Mail.ReadWrite\n  - Mail.Send\n  - MailboxSettings.ReadWrite\n  - Calendars.Read\n  - Calendars.ReadWrite\n  - Files.ReadWrite\n  - Contacts.Read\n  - People.Read\n  how_to_obtain: Register an app in Microsoft Azure Portal, then copy the Application (client) ID, Directory (tenant) ID (if single‑tenant), and\n    client secret into the .env file as MICROSOFT_CLIENT_ID, MICROSOFT_TENANT_ID, and MICROSOFT_CLIENT_SECRET.\ndocs: https://docs.getinboxzero.com/essentials/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/getinboxzero-com/authentication/getinboxzero-com-authentication.yml
summary_line: 2 schemes
tags:
- Email Management
- AI Assistant
- Email Automation
- Open Source
---
