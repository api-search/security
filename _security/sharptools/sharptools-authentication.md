---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sharptools-openapi-generated.yml
  format: yaml
  label: SharpTools API
  slug: sharptools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharptools/openapi/_ae-authored/sharptools-openapi-generated.yml
auth_types: []
description: Authentication methods for connecting external notification services to SharpTools.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Sharptools Authentication
name_suffix: Authentication
oauth_flows: []
overview: SharpTools declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: SharpTools
provider_slug: sharptools
scheme_count: 4
schemes:
- evidence: Copy your User Token from your Pushover account
  how_to_obtain: Create a Pushover account and an application, then copy the User Token displayed in your Pushover account.
  name: Pushover User Token
  type: apiKey
- evidence: Copy your Application/API Key from the Pushover Application page
  how_to_obtain: Create a Pushover application and copy the API Key shown on the application page.
  name: Pushover Application/API Key
  type: apiKey
- evidence: Copy your SID and Auth Token from your Twilio console into the Account SID and Auth Token fields in SharpTools
  how_to_obtain: Create a Twilio account, then retrieve the Account SID from the Twilio console.
  name: Twilio Account SID
  type: apiKey
- evidence: Copy your SID and Auth Token from your Twilio console into the Account SID and Auth Token fields in SharpTools
  how_to_obtain: Create a Twilio account, then retrieve the Auth Token from the Twilio console (may need to click 'view').
  name: Twilio Auth Token
  type: apiKey
slug: sharptools-authentication
source_filename: sharptools-authentication.yml
source_heading: Authentication Profile
source_url: https://help.sharptools.io/article/42-how-do-i-setup-pushover
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.sharptools.io/article/42-how-do-i-setup-pushover\nsources:\n- https://help.sharptools.io/article/42-how-do-i-setup-pushover\n- https://help.sharptools.io/article/44-how-to-setup-notifications\n- https://help.sharptools.io/article/43-how-do-i-setup-twilio-sms\ndescription: Authentication methods for connecting external notification services to SharpTools.\nschemes:\n- type: apiKey\n  name: Pushover User Token\n  evidence: Copy your User Token from your Pushover account\n  how_to_obtain: Create a Pushover account and an application, then copy the User Token displayed in your Pushover account.\n- type: apiKey\n  name: Pushover Application/API Key\n  evidence: Copy your Application/API Key from the Pushover Application page\n  how_to_obtain: Create a Pushover application and copy the API Key shown on the application page.\n- type: apiKey\n  name: Twilio Account SID\n  evidence:\
  \ Copy your SID and Auth Token from your Twilio console into the Account SID and Auth Token fields in SharpTools\n  how_to_obtain: Create a Twilio account, then retrieve the Account SID from the Twilio console.\n- type: apiKey\n  name: Twilio Auth Token\n  evidence: Copy your SID and Auth Token from your Twilio console into the Account SID and Auth Token fields in SharpTools\n  how_to_obtain: Create a Twilio account, then retrieve the Auth Token from the Twilio console (may need to click 'view').\ndocs: https://help.sharptools.io/article/42-how-do-i-setup-pushover\n"
source_yaml_url: https://artifacts.apis.io/sharptools/authentication/sharptools-authentication.yml
summary_line: 4 schemes
tags:
- Smart Home
- Dashboards
- Automation
- Rule Engine
- Hub Integration
- Device Monitoring
- Custom Tiles
---
