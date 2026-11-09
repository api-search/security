---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Okapi Bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Okapi declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Okapi
provider_slug: okapi-bot
scheme_count: 1
schemes:
- description: The documented public JSON (https://www.okapi.bot/api/v1/providers/<provider>.json) and feeds (/breaking-changes/feed.xml, feed.atom, feed.json, calendar.ics) answered unauthenticated GETs with 200 on 2026-11-05. No credential scheme is documented.
  type: none
slug: okapi-bot-authentication
source_filename: okapi-bot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: https://www.okapi.bot/api/v1/providers/100ms-api.json\ndocs: https://www.okapi.bot/llms.txt\nschemes:\n- type: none\n  description: The documented public JSON (https://www.okapi.bot/api/v1/providers/<provider>.json) and feeds (/breaking-changes/feed.xml, feed.atom, feed.json, calendar.ics) answered unauthenticated GETs with 200 on 2026-11-05. No credential scheme is documented.\nnote: The check API named in the terms is available only by emailing hello@okapi.bot; its authentication is not documented. The GitHub App itself is installed through GitHub (https://github.com/apps/okapi-agent).\n"
source_yaml_url: https://artifacts.apis.io/okapi-bot/authentication/okapi-bot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API Change Management
- Breaking Changes
- Deprecation
- GitHub App
- Developer Tools
- API Monitoring
- AI Agents
---
