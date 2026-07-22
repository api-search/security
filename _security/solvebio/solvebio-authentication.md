---
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Solvebio Authentication
name_suffix: Authentication
oauth_flows: []
overview: SolveBio secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SolveBio
provider_slug: solvebio
scheme_count: 3
schemes:
- description: OAuth2 access token supplied via the SOLVEBIO_ACCESS_TOKEN environment variable (or programmatically). Preferred credential.
  env: SOLVEBIO_ACCESS_TOKEN
  name: OAuth2AccessToken
  type: oauth2
- description: API key supplied via SOLVEBIO_API_KEY, sent as an Authorization token header to the API host.
  env: SOLVEBIO_API_KEY
  in: header
  name: ApiKey
  type: apiKey
- description: '`solvebio login` prompts for credentials and caches a token in the local credentials file (~/.solvebio).'
  name: InteractiveLogin
  scheme: credentials
  type: http
slug: solvebio-authentication
source_filename: solvebio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/solvebio/solvebio-python\ndocs: https://github.com/solvebio/solvebio-python#configuring-the-client\nnote: >-\n  Derived from the first-party client documentation (no public OpenAPI is\n  reachable — the QuartzBio EDP REST API is served per-customer at instance\n  hosts such as https://solvebio.api.az.aws.quartz.bio with a Swagger UI at\n  {api_host}/swagger behind authentication).\nsummary:\n  types: [oauth2, apiKey]\n  credential_lookup_order:\n    - access_token   # SOLVEBIO_ACCESS_TOKEN (OAuth2)\n    - api_key        # SOLVEBIO_API_KEY\n    - local_credentials_file  # solvebio login\nschemes:\n  - name: OAuth2AccessToken\n    type: oauth2\n    description: >-\n      OAuth2 access token supplied via the SOLVEBIO_ACCESS_TOKEN environment\n      variable (or programmatically). Preferred credential.\n    env: SOLVEBIO_ACCESS_TOKEN\n  - name: ApiKey\n    type: apiKey\n    in: header\n    description: >-\n \
  \     API key supplied via SOLVEBIO_API_KEY, sent as an Authorization token\n      header to the API host.\n    env: SOLVEBIO_API_KEY\n  - name: InteractiveLogin\n    type: http\n    scheme: credentials\n    description: >-\n      `solvebio login` prompts for credentials and caches a token in the local\n      credentials file (~/.solvebio).\nconfig_env:\n  api_host: SOLVEBIO_API_HOST\n  access_token: SOLVEBIO_ACCESS_TOKEN\n  api_key: SOLVEBIO_API_KEY\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solvebio/refs/heads/main/authentication/solvebio-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Company
- Genomics
- Bioinformatics
- Life Sciences
- Precision Medicine
- Biomedical Data
- Datasets
- SDK
---
