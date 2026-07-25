---
api_key_in:
- header
api_specs:
- filename: have-i-been-pwned-breach-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Breach API
  slug: have-i-been-pwned-breach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-breach-api-openapi.yml
- filename: have-i-been-pwned-breachedaccount-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Breachedaccount API
  slug: have-i-been-pwned-breachedaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-breachedaccount-api-openapi.yml
- filename: have-i-been-pwned-breacheddomain-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Breacheddomain API
  slug: have-i-been-pwned-breacheddomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-breacheddomain-api-openapi.yml
- filename: have-i-been-pwned-breaches-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Breaches API
  slug: have-i-been-pwned-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-breaches-api-openapi.yml
- filename: have-i-been-pwned-dataclasses-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Dataclasses API
  slug: have-i-been-pwned-dataclasses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-dataclasses-api-openapi.yml
- filename: have-i-been-pwned-domainverification-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Domainverification API
  slug: have-i-been-pwned-domainverification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-domainverification-api-openapi.yml
- filename: have-i-been-pwned-latestbreach-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Latestbreach API
  slug: have-i-been-pwned-latestbreach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-latestbreach-api-openapi.yml
- filename: have-i-been-pwned-pasteaccount-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Pasteaccount API
  slug: have-i-been-pwned-pasteaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-pasteaccount-api-openapi.yml
- filename: have-i-been-pwned-range-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Range API
  slug: have-i-been-pwned-range-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-range-api-openapi.yml
- filename: have-i-been-pwned-stealerlogsbyemail-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Stealerlogsbyemail API
  slug: have-i-been-pwned-stealerlogsbyemail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-stealerlogsbyemail-api-openapi.yml
- filename: have-i-been-pwned-stealerlogsbyemaildomain-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Stealerlogsbyemaildomain API
  slug: have-i-been-pwned-stealerlogsbyemaildomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-stealerlogsbyemaildomain-api-openapi.yml
- filename: have-i-been-pwned-stealerlogsbywebsitedomain-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Stealerlogsbywebsitedomain API
  slug: have-i-been-pwned-stealerlogsbywebsitedomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-stealerlogsbywebsitedomain-api-openapi.yml
- filename: have-i-been-pwned-subscribeddomains-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Subscribeddomains API
  slug: have-i-been-pwned-subscribeddomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-subscribeddomains-api-openapi.yml
- filename: have-i-been-pwned-subscription-api-openapi.yml
  format: yaml
  label: Have I Been Pwned Subscription API
  slug: have-i-been-pwned-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-subscription-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Have I Been Pwned Authentication
name_suffix: Authentication
oauth_flows: []
overview: Have I Been Pwned secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Have I Been Pwned
provider_slug: have-i-been-pwned
scheme_count: 1
schemes:
- description: HIBP API key passed in the hibp-api-key header. Paid APIs require a 32-character hexadecimal value. On supported test-only endpoints, any 32-character hexadecimal value can be used as a test key for the hibp-integration-tests.com domain.
  in: header
  name: HibpApiKey
  parameter: hibp-api-key
  sources:
  - openapi/have-i-been-pwned-openapi.json
  type: apiKey
slug: have-i-been-pwned-authentication
source_filename: have-i-been-pwned-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/have-i-been-pwned-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HibpApiKey\n  type: apiKey\n  in: header\n  parameter: hibp-api-key\n  description: HIBP API key passed in the hibp-api-key header. Paid APIs require a 32-character\n    hexadecimal value. On supported test-only endpoints, any 32-character hexadecimal value\n    can be used as a test key for the hibp-integration-tests.com domain.\n  sources:\n  - openapi/have-i-been-pwned-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/authentication/have-i-been-pwned-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Data Breaches
- Pwned Passwords
- Identity
- Threat Intelligence
- Credential Stuffing
---
