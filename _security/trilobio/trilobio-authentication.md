---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Trilobio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trilobio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Trilobio
provider_slug: trilobio
scheme_count: 1
schemes:
- evidence: '"Note that the TCodeServicerClient constructor is called with no arguments. By default, it connects to the T-code Servicer running on the local [machine]." Trust boundary is physical/network access to the fleet control computer, not credential-based.'
  scope: local-loopback
  type: none
slug: trilobio-authentication
source_filename: trilobio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: 'http://tcode.trilo.bio/ (Tutorial: Connecting to a Trilobio Fleet) + README'\napi: tcode-api\nsummary: >-\n  The tcode-api is a local, on-premises control API rather than an\n  internet-facing REST service. Scripts run on the fleet control computer and\n  talk to the T-code Servicer over the loopback interface. The\n  `TCodeServicerClient()` constructor is called with no arguments and, by\n  default, connects to the T-code Servicer running on the local machine — there\n  are no API keys, OAuth flows, or bearer tokens documented for the client.\nschemes:\n- type: none\n  scope: local-loopback\n  evidence: >-\n    \"Note that the TCodeServicerClient constructor is called with no arguments.\n    By default, it connects to the T-code Servicer running on the local\n    [machine].\" Trust boundary is physical/network access to the fleet control\n    computer, not credential-based.\nnetwork_auth: none\nnotes: >-\n  No OAuth2/OpenID\
  \ Connect/apiKey/mutualTLS security schemes are declared or\n  documented. Access control is effected by controlling access to the fleet\n  control computer on which the T-code Servicer runs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trilobio/refs/heads/main/authentication/trilobio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Frontier Tech
- Lab Automation
- Biotech
- Life Sciences
- Robotics
- Synthetic Biology
- Developer API
- Python SDK
---
