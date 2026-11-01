---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sleeperhit Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: sleeperhit-studio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: sleeperhit-studio
provider_slug: sleeperhit-studio
scheme_count: 1
schemes:
- bearerFormat: Sleeper Hit API key (sh_<prefix>_<secret>)
  description: Production-only customer API key. Created and revoked at https://sleeperhit.studio/dashboard/developers. Tokens are shown once; store them in your secret manager.
  scheme: bearer
  type: http
slug: sleeperhit-studio-authentication
source_filename: sleeperhit-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://docs.sleeperhit.studio/api-reference\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: \"Sleeper Hit API key (sh_<prefix>_<secret>)\"\n    description: \"Production-only customer API key. Created and revoked at https://sleeperhit.studio/dashboard/developers. Tokens are shown once; store them in your secret manager.\"\n"
source_yaml_url: https://artifacts.apis.io/sleeperhit-studio/authentication/sleeperhit-studio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Audio
- Video
- Podcast
- Enterprise
- Automation
---
