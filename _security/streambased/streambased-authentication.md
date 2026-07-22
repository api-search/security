---
api_key_in:
- credential
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Streambased Authentication
name_suffix: Authentication
oauth_flows: []
overview: Streambased secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Streambased
provider_slug: streambased
scheme_count: 1
schemes:
- description: Per-cluster Streambased API Key that authenticates requests to Streambased managed services. Created in Streambased Cloud under the Kafka cluster.
  in: credential
  name: StreambasedApiKey
  sources:
  - https://docs.streambased.io/deploy-and-operate/streambased-cloud/create-your-first-streambased-api-key
  type: apiKey
slug: streambased-authentication
source_filename: streambased-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.streambased.io/deploy-and-operate/streambased-cloud/create-your-first-streambased-api-key\ndocs: https://docs.streambased.io/deploy-and-operate/streambased-cloud/create-your-first-streambased-api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - credential\n  oauth2_flows: []\n  note: >-\n    Streambased Cloud authenticates requests with a Streambased API Key. An API\n    Key is created per Kafka cluster and authenticates access to Streambased\n    managed services (the Iceberg REST interface / SQL query surface over your\n    Kafka topics). Streambased is consumed through standard Apache Kafka and\n    Apache Iceberg REST clients rather than a bespoke REST API, so the API key is\n    supplied through the client's credential mechanism (e.g. Kafka SASL / Iceberg\n    catalog credential) rather than a documented HTTP header name.\nschemes:\n- name: StreambasedApiKey\n  type: apiKey\n  in: credential\n  description:\
  \ >-\n    Per-cluster Streambased API Key that authenticates requests to Streambased\n    managed services. Created in Streambased Cloud under the Kafka cluster.\n  sources:\n  - https://docs.streambased.io/deploy-and-operate/streambased-cloud/create-your-first-streambased-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streambased/refs/heads/main/authentication/streambased-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Streaming
- Apache Kafka
- Apache Iceberg
- Analytics
- Real-Time Data
- Data Lakehouse
- SQL
- Data Governance
---
