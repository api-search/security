---
anonymous_access: true
api_key_in: []
api_specs:
- filename: mailsenpai-account-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Account API
  slug: mailsenpai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-account-api-openapi.yml
- filename: mailsenpai-log-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Log API
  slug: mailsenpai-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-log-api-openapi.yml
- filename: mailsenpai-sending-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Sending API
  slug: mailsenpai-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-sending-api-openapi.yml
- filename: mailsenpai-suppression-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Suppression API
  slug: mailsenpai-suppression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-suppression-api-openapi.yml
- filename: mailsenpai-webhooks-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Webhooks API
  slug: mailsenpai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-webhooks-api-openapi.yml
- filename: mailsenpai-website-forms-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Website forms API
  slug: mailsenpai-website-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailsenpai/openapi/mailsenpai-website-forms-api-openapi.yml
auth_types: []
description: Authentication methods as published by the provider, per surface. The transactional REST API, the SMTP relay, the public diagnostic APIs and the marketing-platform MCP server each authenticate differently.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: SMTP Senpai (MailSenpai) Authentication
name_suffix: Authentication
oauth_flows: []
overview: SMTP Senpai (MailSenpai) declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: SMTP Senpai (MailSenpai)
provider_slug: mailsenpai
scheme_count: 4
schemes:
- applies_to: SMTP Senpai transactional REST API (OpenAPI 3.1.0, v1.2.0)
  evidence: 'securitySchemes.chiaveBearer: `Authorization: Bearer msp_…` (the key starts with `msp_`). As an alternative the `chiave` field is accepted in the body (JSON or form). A key in the URL (`?chiave=`) is refused with 401.'
  how_to_obtain: API key (prefix msp_) from the SMTP Senpai user area.
  location: header
  name: SMTP Senpai REST API key
  scheme: bearer
  type: http
- applies_to: SMTP relay transport only -- separate from the REST API
  evidence: SMTP credentials are provided in the user area (SMTP Senpai page; Microsoft 365 SMTP tutorial).
  how_to_obtain: Username and password from the SMTP Senpai user area.
  location: smtp
  name: SMTP AUTH (username/password)
  type: other
- applies_to: Public diagnostic APIs -- DNS check API (https://en.mailsenpai.com/dns-check-api/) and blacklist check API (https://en.mailsenpai.com/blacklist-check-api/)
  evidence: Listed in https://en.mailsenpai.com/apis.json as keyless public APIs; they do not inherit the REST API bearer requirement.
  name: No authentication
  type: none
- applies_to: MailSenpai marketing-platform MCP server at https://mcp.mailsenpai.com/mcp -- a separate service from the SMTP Senpai REST API
  evidence: Documented at https://mcp.mailsenpai.com/docs
  how_to_obtain: OAuth sign-in with a MailSenpai account.
  name: MailSenpai MCP server (OAuth)
  type: oauth2
slug: mailsenpai-authentication
source_filename: mailsenpai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mailsenpai.com/wp-content/uploads/api/smtp-senpai-openapi-1.2.0.en.json
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: support correction (email, 2026-10-19 request from MailSenpai), verified against the provider's own OpenAPI\nsource: https://www.mailsenpai.com/wp-content/uploads/api/smtp-senpai-openapi-1.2.0.en.json\nsources:\n- https://www.mailsenpai.com/wp-content/uploads/api/smtp-senpai-openapi-1.2.0.en.json\n- https://en.mailsenpai.com/smtp-senpai/\n- https://en.mailsenpai.com/apis.json\n- https://mcp.mailsenpai.com/docs\ndescription: Authentication methods as published by the provider, per surface. The transactional REST API, the SMTP relay, the public diagnostic APIs and the marketing-platform MCP server each authenticate differently.\nschemes:\n- type: http\n  scheme: bearer\n  name: SMTP Senpai REST API key\n  applies_to: SMTP Senpai transactional REST API (OpenAPI 3.1.0, v1.2.0)\n  evidence: 'securitySchemes.chiaveBearer: `Authorization: Bearer msp_…` (the key starts with `msp_`). As an alternative the `chiave` field is accepted\
  \ in the body (JSON or form). A key in the URL (`?chiave=`) is refused with 401.'\n  location: header\n  how_to_obtain: API key (prefix msp_) from the SMTP Senpai user area.\n- type: other\n  name: SMTP AUTH (username/password)\n  applies_to: SMTP relay transport only -- separate from the REST API\n  evidence: SMTP credentials are provided in the user area (SMTP Senpai page; Microsoft 365 SMTP tutorial).\n  location: smtp\n  how_to_obtain: Username and password from the SMTP Senpai user area.\n- type: none\n  name: No authentication\n  applies_to: Public diagnostic APIs -- DNS check API (https://en.mailsenpai.com/dns-check-api/) and blacklist check API (https://en.mailsenpai.com/blacklist-check-api/)\n  evidence: Listed in https://en.mailsenpai.com/apis.json as keyless public APIs; they do not inherit the REST API bearer requirement.\n- type: oauth2\n  name: MailSenpai MCP server (OAuth)\n  applies_to: MailSenpai marketing-platform MCP server at https://mcp.mailsenpai.com/mcp -- a separate\
  \ service from the SMTP Senpai REST API\n  evidence: Documented at https://mcp.mailsenpai.com/docs\n  how_to_obtain: OAuth sign-in with a MailSenpai account.\ndocs: https://www.mailsenpai.com/wp-content/uploads/api/smtp-senpai-openapi-1.2.0.en.json\n"
source_yaml_url: https://artifacts.apis.io/mailsenpai/authentication/mailsenpai-authentication.yml
summary_line: 4 schemes
tags:
- Email Marketing
- B2B outreach
- SMTP relay
- Artificial Intelligence
- Newsletter platform
---
