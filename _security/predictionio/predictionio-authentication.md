---
api_key_in: []
auth_types: []
description: Authentication profile for the Apache PredictionIO Event Server REST API. The Event Server authenticates requests with a per-app access key. Engine query endpoints are unauthenticated by default and rely on network-level controls.
kind: authentication
layout: security
method: searched
name: Predictionio Authentication
name_suffix: Authentication
oauth_flows: []
overview: PredictionIO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PredictionIO
provider_slug: predictionio
scheme_count: 2
schemes:
- applies_to: Event Server API (localhost:7070)
  description: 'Per-application access key passed as the `accessKey` query parameter on every Event Server request. Generated when an app is created via the CLI command `pio app new`. Example: /events.json?accessKey=yourAccessKeyString'
  id: accessKey
  in: query
  name: accessKey
  type: apiKey
- applies_to: Engine Query API (localhost:8000)
  description: The deployed prediction engine query endpoint (POST /queries.json) has no built-in authentication; access is expected to be restricted at the network or gateway layer.
  id: none
  type: none
slug: predictionio-authentication
source_filename: predictionio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://predictionio.apache.org/datacollection/eventapi/ (2026-07-20)\nname: PredictionIO Authentication\ndescription: >-\n  Authentication profile for the Apache PredictionIO Event Server REST API. The\n  Event Server authenticates requests with a per-app access key. Engine query\n  endpoints are unauthenticated by default and rely on network-level controls.\ndocs: https://predictionio.apache.org/datacollection/eventapi/\nschemes:\n- id: accessKey\n  type: apiKey\n  in: query\n  name: accessKey\n  applies_to: Event Server API (localhost:7070)\n  description: >-\n    Per-application access key passed as the `accessKey` query parameter on every\n    Event Server request. Generated when an app is created via the CLI command\n    `pio app new`. Example: /events.json?accessKey=yourAccessKeyString\n- id: none\n  type: none\n  applies_to: Engine Query API (localhost:8000)\n  description: >-\n    The deployed prediction engine query\
  \ endpoint (POST /queries.json) has no\n    built-in authentication; access is expected to be restricted at the network\n    or gateway layer.\nnotes: >-\n  No OAuth2, OpenID Connect, or mutual TLS is documented. The access key is an\n  opaque application credential, not an OAuth token, so no scopes apply.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predictionio/refs/heads/main/authentication/predictionio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Machine Learning
- Artificial Intelligence
- Predictive Analytics
- Recommendation Engine
- Open Source
- Apache
- Event Server
- Retired
---
