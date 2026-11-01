---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for sending emails via Paradigm uses OAuth to connect a user's email provider (Google or Microsoft).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Paradigmai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paradigm declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Paradigm
provider_slug: paradigmai-com
scheme_count: 1
schemes:
- evidence: When you attempt to send emails for the first time, you'll see a prompt to connect your account. Click `Connect OAuth`.
  flows:
  - authorization_code
  how_to_obtain: Click the **Connect OAuth** button, select your email provider (Google or Microsoft), and approve the requested permissions on the provider’s authorization page.
  name: OAuth
  type: oauth2
slug: paradigmai-com-authentication
source_filename: paradigmai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.paradigmai.com/email/email-setup.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.paradigmai.com/email/email-setup.md\nsources:\n- https://docs.paradigmai.com/email/email-setup.md\n- https://docs.paradigmai.com/getting-started/intro.md\n- https://docs.paradigmai.com/sheet-setup/templates.md\n- https://docs.paradigmai.com/sheet-setup/blank-sheet.md\ndescription: Authentication for sending emails via Paradigm uses OAuth to connect a user's email provider (Google or Microsoft).\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: When you attempt to send emails for the first time, you'll see a prompt to connect your account. Click `Connect OAuth`.\n  flows:\n  - authorization_code\n  how_to_obtain: Click the **Connect OAuth** button, select your email provider (Google or Microsoft), and approve the requested permissions on\n    the provider’s authorization page.\ndocs: https://docs.paradigmai.com/email/email-setup.md\n"
source_yaml_url: https://artifacts.apis.io/paradigmai-com/authentication/paradigmai-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- GTM
- Automation
- Analytics
---
