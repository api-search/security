---
anonymous_access: false
api_key_in: []
api_specs:
- filename: franklymail-com-openapi-generated.yml
  format: yaml
  label: FranklyMail API
  slug: franklymail-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/franklymail-com/openapi/_ae-authored/franklymail-com-openapi-generated.yml
auth_types: []
description: Authentication methods published on FranklyMail documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FranklyMail Authentication
name_suffix: Authentication
oauth_flows: []
overview: FranklyMail declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FranklyMail
provider_slug: franklymail-com
scheme_count: 2
schemes:
- evidence: Enter your full mailbox email address as the username and the app password created for that mailbox as the password.
  header: Authorization
  how_to_obtain: Create an app password under Settings → App passwords in the FranklyMail dashboard and use it as the password with your full mailbox email address as the username.
  location: header
  name: JMAP login
  type: http-basic
- evidence: Sign in to your own mailbox through webmail to connect.
  how_to_obtain: Sign in to your own mailbox through webmail and grant permission when the FranklyMail permission screen appears.
  name: Agentic Inbox
  type: oauth2
slug: franklymail-com-authentication
source_filename: franklymail-com-authentication.yml
source_heading: Authentication Profile
source_url: https://franklymail.com/guides/jmap
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://franklymail.com/guides/jmap\nsources:\n- https://franklymail.com/guides/jmap\n- https://franklymail.com/docs/agentic-inbox\n- https://franklymail.com/nl/docs/agentic-inbox\ndescription: Authentication methods published on FranklyMail documentation pages.\nschemes:\n- type: http-basic\n  name: JMAP login\n  evidence: Enter your full mailbox email address as the username and the app password created for that mailbox as the password.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an app password under Settings → App passwords in the FranklyMail dashboard and use it as the password with your full\n    mailbox email address as the username.\n- type: oauth2\n  name: Agentic Inbox\n  evidence: Sign in to your own mailbox through webmail to connect.\n  how_to_obtain: Sign in to your own mailbox through webmail and grant permission when the FranklyMail permission\
  \ screen appears.\ndocs: https://franklymail.com/guides/jmap\n"
source_yaml_url: https://artifacts.apis.io/franklymail-com/authentication/franklymail-com-authentication.yml
summary_line: 2 schemes
tags:
- Email
- Collaboration
- Software-as-a-Service
- Small Business
- Privacy
---
