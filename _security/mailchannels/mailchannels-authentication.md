---
anonymous_access: false
api_key_in: []
auth_types: []
description: MailChannels uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailchannels Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailChannels declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MailChannels
provider_slug: mailchannels
scheme_count: 1
schemes:
- evidence: Every request to the Email API must include your API key.
  header: X-Api-Key
  how_to_obtain: Create an API key in the MailChannels Console (see the “Creating an API key” section) or via the parent‑account sub‑account endpoints.
  location: header
  name: X-Api-Key
  type: apiKey
slug: mailchannels-authentication
source_filename: mailchannels-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mailchannels.com/api-reference/sub-accounts/retrieve-sub-account-api-keys.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mailchannels.com/api-reference/sub-accounts/retrieve-sub-account-api-keys.md\nsources:\n- https://docs.mailchannels.com/api-reference/sub-accounts/retrieve-sub-account-api-keys.md\n- https://docs.mailchannels.com/api-reference/sub-accounts/create-sub-account-api-key.md\n- https://docs.mailchannels.com/api-reference/sub-accounts/delete-sub-account-api-key.md\n- https://docs.mailchannels.com/email-api/authentication.md\ndescription: MailChannels uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: Every request to the Email API must include your API key.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create an API key in the MailChannels Console (see the “Creating an API key” section) or via the parent‑account sub‑account endpoints.\ndocs: https://docs.mailchannels.com/api-reference/sub-accounts/retrieve-sub-account-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/mailchannels/authentication/mailchannels-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- API
- SMTP
- Platform
---
