---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailsenpai-account-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Account API
  slug: mailsenpai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-account-api-openapi.yml
- filename: mailsenpai-log-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Log API
  slug: mailsenpai-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-log-api-openapi.yml
- filename: mailsenpai-sending-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Sending API
  slug: mailsenpai-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-sending-api-openapi.yml
- filename: mailsenpai-smtp-senpai-api-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) SMTP Senpai API
  slug: mailsenpai-smtp-senpai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-smtp-senpai-api-api-openapi.yml
- filename: mailsenpai-suppression-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Suppression API
  slug: mailsenpai-suppression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-suppression-api-openapi.yml
- filename: mailsenpai-webhooks-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Webhooks API
  slug: mailsenpai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-webhooks-api-openapi.yml
- filename: mailsenpai-website-forms-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Website forms API
  slug: mailsenpai-website-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-website-forms-api-openapi.yml
auth_types: []
description: Authentication methods as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailsenpai Authentication
name_suffix: Authentication
oauth_flows: []
overview: SMTP Senpai (MailSenpai) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SMTP Senpai (MailSenpai)
provider_slug: mailsenpai
scheme_count: 1
schemes:
- evidence: Accesso utente e password Utente dalla tua area
  how_to_obtain: Username and password are provided in the user area of MailSenpai.
  location: body
  name: SMTP AUTH (username/password)
  type: other
slug: mailsenpai-authentication
source_filename: mailsenpai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mailsenpai.com/smtp-microsoft-365/
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mailsenpai.com/smtp-microsoft-365/\nsources:\n- https://www.mailsenpai.com/smtp-microsoft-365/\ndescription: Authentication methods as published on the page.\nschemes:\n- type: other\n  name: SMTP AUTH (username/password)\n  evidence: Accesso utente e password Utente dalla tua area\n  location: body\n  how_to_obtain: Username and password are provided in the user area of MailSenpai.\ndocs: https://www.mailsenpai.com/smtp-microsoft-365/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/authentication/mailsenpai-authentication.yml
summary_line: 1 scheme
tags:
- Email marketing
- B2B outreach
- SMTP relay
- Artificial intelligence
- Newsletter platform
---
