---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hello-audio-hello-audio-api-api-openapi.yml
  format: yaml
  label: Hello Audio API
  slug: hello-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hello-audio/openapi/hello-audio-hello-audio-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hello Audio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hello Audio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hello Audio
provider_slug: hello-audio
scheme_count: 2
schemes:
- description: Per-feed webhook URLs carry the account's API key inside the URL itself. The docs say "Treat your API Key inside the webhook URL like your password. Do not share it with anyone. You can click Regenerate to erase the old one and start fresh. This disables all old webhook URLs."
  evidence: https://help.helloaudio.fm/en/articles/10260476-activecampaign-webhook-urls
  in: url
  name: webhook-url-api-key
  rotation: Regenerate on the Integrations page; regenerating invalidates every previously issued webhook URL.
  type: apiKey
- description: The Zapier app connects by signing in to a Hello Audio account inside Zapier ("it will ask you to sign in to your Hello Audio account to connect it to Zapier. You'll only do that once."). The docs do not name the underlying mechanism (OAuth or key).
  evidence: https://help.helloaudio.fm/en/articles/10260487-getting-started-with-zapier
  name: zapier-account-connection
  type: platform-connection
slug: hello-audio-authentication
source_filename: hello-audio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://help.helloaudio.fm/en/articles/10260476-activecampaign-webhook-urls\ndocs: https://help.helloaudio.fm/en/articles/10260476-activecampaign-webhook-urls\nnote: Hello Audio publishes no REST API or OpenAPI. The only documented programmatic entry points are per-feed inbound webhook URLs\n  (copied from https://app.helloaudio.fm/integrations) and the Zapier app. Nothing here was called; it records what the help center says.\nschemes:\n- name: webhook-url-api-key\n  type: apiKey\n  in: url\n  description: Per-feed webhook URLs carry the account's API key inside the URL itself. The docs say \"Treat your API Key inside the webhook\n    URL like your password. Do not share it with anyone. You can click Regenerate to erase the old one and start fresh. This disables all\n    old webhook URLs.\"\n  rotation: Regenerate on the Integrations page; regenerating invalidates every previously issued webhook URL.\n  evidence: https://help.helloaudio.fm/en/articles/10260476-activecampaign-webhook-urls\n\
  - name: zapier-account-connection\n  type: platform-connection\n  description: The Zapier app connects by signing in to a Hello Audio account inside Zapier (\"it will ask you to sign in to your Hello Audio\n    account to connect it to Zapier. You'll only do that once.\"). The docs do not name the underlying mechanism (OAuth or key).\n  evidence: https://help.helloaudio.fm/en/articles/10260487-getting-started-with-zapier\n"
source_yaml_url: https://artifacts.apis.io/hello-audio/authentication/hello-audio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Audio
- Podcast
- SaaS
- Private
- Private Podcasts
- Webhooks
- Zapier
- Creator Economy
---
