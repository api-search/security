---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Replicon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Replicon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Replicon
provider_slug: replicon
scheme_count: 2
schemes:
- description: Personal access token created under Account > Access Tokens in Polaris. The `Api-token` header is required on every Polaris API call. Tokens expire if unused for 30 days.
  in: header
  name: PolarisAccessToken
  parameter_name: Api-token
  source: https://learning.deltek.com/bundle/Replicon/page/setting-up-a-replicon-or-polaris-api-account.html
  type: apiKey
- description: Replicon web services accept HTTP Basic authentication using the tenant company key plus a user login and password (service-account recommended).
  name: HTTPBasic
  scheme: basic
  source: https://www.replicon.com/help/getting-started-with-the-replicon-and-polaris-api/
  type: http
slug: replicon-authentication
source_filename: replicon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://learning.deltek.com/bundle/Replicon/page/getting-started-with-the-replicon-and-polaris-api.html\ndocs: https://www.replicon.com/help/getting-started-with-the-replicon-and-polaris-api/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  notes: >-\n    Replicon and Polaris expose a proprietary JSON-over-HTTP web-service API (no\n    public OpenAPI). Callers first resolve their tenant's swimlane (regional\n    service host, e.g. na1/eu1/sb1.replicon.com) via the global discovery\n    service, then authenticate every call with a token or HTTP Basic credentials.\nschemes:\n  - name: PolarisAccessToken\n    type: apiKey\n    in: header\n    parameter_name: Api-token\n    description: >-\n      Personal access token created under Account > Access Tokens in Polaris.\n      The `Api-token` header is required on every Polaris API call. Tokens expire\n      if unused for 30 days.\n    source: https://learning.deltek.com/bundle/Replicon/page/setting-up-a-replicon-or-polaris-api-account.html\n\
  \  - name: HTTPBasic\n    type: http\n    scheme: basic\n    description: >-\n      Replicon web services accept HTTP Basic authentication using the tenant\n      company key plus a user login and password (service-account recommended).\n    source: https://www.replicon.com/help/getting-started-with-the-replicon-and-polaris-api/\ndiscovery:\n  service: https://global.replicon.com/DiscoveryService1.svc/GetTenantEndpointDetails\n  input: companyKey\n  purpose: >-\n    Returns the tenant's regional service endpoint (swimlane). Clients must call\n    this to determine the correct host before issuing authenticated API calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicon/refs/heads/main/authentication/replicon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Enterprise Software
- Time Tracking
- Timesheets
- Project Management
- Professional Services Automation
- Workforce Management
- Billing
---
