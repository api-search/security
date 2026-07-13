---
api_key_in:
- header
api_specs:
- filename: mist-ai-openapi.yml
  format: yaml
  label: Juniper Mist Cloud API
  slug: juniper-mist-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mist-ai/refs/heads/main/openapi/mist-ai-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mist Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juniper Mist AI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Juniper Mist AI
provider_slug: mist-ai
scheme_count: 3
schemes:
- description: "Like many other API providers, it’s also possible to generate API Tokens to be used (in HTTP Header) for authentication. An API token ties to a Admin with equal or less privileges.\n\n**Format**:\n  API Token value format is `Token {apitoken}`\n\n**Notes**:\n* an API token generated for a specific admin has the same privilege as the user\n* an API token will be automatically removed if not used for > 90 "
  in: header
  name: apiToken
  parameter: Authorization
  sources:
  - openapi/mist-ai-openapi.yml
  type: apiKey
- description: While our current UI uses Session / Cookie-based authentication, it’s also possible to do Basic Auth.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mist-ai-openapi.yml
  type: http
- description: "This protects the website against [Cross Site Request Forgery](https://en.wikipedia.org/wiki/Cross-site_request_forgery), all the POST / PUT / DELETE APIs needs to have CSRF token in the AJAX Request header when using Login/Password authentication (with or without MFA)\n\n\nThe CSRF Token is sent back by Mist in the Cookies from the Login Response API Call:\n`cookies[csrftoken]` \n\nThe CSRF Token must "
  in: header
  name: csrfToken
  parameter: X-CSRFToken
  sources:
  - openapi/mist-ai-openapi.yml
  type: apiKey
slug: mist-ai-authentication
source_filename: mist-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mist-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"Like many other API providers, it’s also possible to generate API Tokens to\\\n    \\ be used (in HTTP Header) for authentication. An API token ties to a Admin with equal or\\\n    \\ less privileges.\\n\\n**Format**:\\n  API Token value format is `Token {apitoken}`\\n\\n**Notes**:\\n\\\n    * an API token generated for a specific admin has the same privilege as the user\\n* an API\\\n    \\ token will be automatically removed if not used for > 90 \"\n  sources:\n  - openapi/mist-ai-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: While our current UI uses Session / Cookie-based authentication, it’s also possible\n    to do Basic Auth.\n  sources:\n  - openapi/mist-ai-openapi.yml\n- name: csrfToken\n\
  \  type: apiKey\n  in: header\n  parameter: X-CSRFToken\n  description: \"This protects the website against [Cross Site Request Forgery](https://en.wikipedia.org/wiki/Cross-site_request_forgery),\\\n    \\ all the POST / PUT / DELETE APIs needs to have CSRF token in the AJAX Request header when\\\n    \\ using Login/Password authentication (with or without MFA)\\n\\n\\nThe CSRF Token is sent\\\n    \\ back by Mist in the Cookies from the Login Response API Call:\\n`cookies[csrftoken]` \\n\\\n    \\nThe CSRF Token must \"\n  sources:\n  - openapi/mist-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mist-ai/refs/heads/main/authentication/mist-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI
- AIOps
- Artificial Intelligence
- Networking
- Wi-Fi
- Wireless LAN
- WAN
- SD-WAN
- Wired
- LAN
- Access Points
- Switches
- Routers
- Marvis
- NAC
- Access Assurance
- Location Services
- Bluetooth LE
- Indoor Location
- Cloud Networking
- Microservices
- Enterprise Networking
- AI Native Networking
---
