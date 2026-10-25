---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Imdex Authentication
name_suffix: Authentication
oauth_flows: []
overview: IMDEX declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IMDEX
provider_slug: imdex
scheme_count: 1
schemes:
- evidence: https://help.seequent.com/Central/en-GB/Content/guides/integrations.htm
  in: null
  name: null
  note: Key created in IMDEXHUB-IQ under Account Management > API Keys and scoped to the IMDEX projects of that account. The docs do not say how the key is transmitted (header or query, and the name), so those fields are left null.
  type: apiKey
slug: imdex-authentication
source_filename: imdex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://help.seequent.com/Central/en-GB/Content/guides/integrations.htm\ndocs: https://help.seequent.com/Central/en-GB/Content/guides/integrations.htm\nsummary: >-\n  IMDEX publishes no public API reference or OpenAPI. The only public description of how to authenticate to the\n  IMDEXHUB-IQ integration API is on a partner page (Seequent Central help). It says keys are self-issued per user:\n  \"click on your username, then on Account Management. Select the API Keys option, then create a new key.\" The page\n  also says a key is bound to IMDEX projects: \"the API key copied from the IMDEXHUB-IQ™ website will allow you to\n  retrieve the IMDEX projects associated with that API key\". No header name, location or scheme is published.\nschemes:\n- type: apiKey\n  name: null\n  in: null\n  note: >-\n    Key created in IMDEXHUB-IQ under Account Management > API Keys and scoped to the IMDEX projects of that account.\n    The docs do\
  \ not say how the key is transmitted (header or query, and the name), so those fields are left null.\n  evidence: https://help.seequent.com/Central/en-GB/Content/guides/integrations.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imdex/refs/heads/main/authentication/imdex-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Mining
- Mining Technology
- Geoscience
- Drilling
- Data Platform
- Australia
---
