---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Adanos Market Sentiment API
  slug: adanos-market-sentiment-api
  spec_type: OpenAPI
  url: https://api.adanos.org/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adanos Market Sentiment Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adanos Market Sentiment API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adanos Market Sentiment API
provider_slug: adanos-market-sentiment-api
scheme_count: 1
schemes:
- description: 'API key for authentication.


    Get your API key at https://adanos.org/register.


    Format: `sk_live_` followed by 32 hexadecimal characters. Example: `REDACTED_STRIPE_KEY`.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/adanos-market-sentiment-api-news-openapi.yaml
  - openapi/adanos-market-sentiment-api-openapi.json
  - openapi/adanos-market-sentiment-api-polymarket-openapi.yaml
  - openapi/adanos-market-sentiment-api-reddit-crypto-openapi.yaml
  - openapi/adanos-market-sentiment-api-reddit-openapi.yaml
  - openapi/adanos-market-sentiment-api-sentiment-openapi.yaml
  - openapi/adanos-market-sentiment-api-x-openapi.yaml
  type: apiKey
slug: adanos-market-sentiment-api-authentication
source_filename: adanos-market-sentiment-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/adanos-market-sentiment-api-news-openapi.yaml, openapi/adanos-market-sentiment-api-openapi.json,\n  openapi/adanos-market-sentiment-api-polymarket-openapi.yaml, openapi/adanos-market-sentiment-api-reddit-crypto-openapi.yaml,\n  openapi/adanos-market-sentiment-api-reddit-openapi.yaml, openapi/adanos-market-sentiment-api-sentiment-openapi.yaml,\n  openapi/adanos-market-sentiment-api-x-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key for authentication.\n\n    Get your API key at https://adanos.org/register.\n\n    Format: `sk_live_` followed by 32 hexadecimal characters. Example: `REDACTED_STRIPE_KEY`.\n  sources:\n  - openapi/adanos-market-sentiment-api-news-openapi.yaml\n  - openapi/adanos-market-sentiment-api-openapi.json\n  - openapi/adanos-market-sentiment-api-polymarket-openapi.yaml\n\
  \  - openapi/adanos-market-sentiment-api-reddit-crypto-openapi.yaml\n  - openapi/adanos-market-sentiment-api-reddit-openapi.yaml\n  - openapi/adanos-market-sentiment-api-sentiment-openapi.yaml\n  - openapi/adanos-market-sentiment-api-x-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adanos-market-sentiment-api/refs/heads/main/authentication/adanos-market-sentiment-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Market
- Sentiment
- Stocks
- Crypto
- Finance
- Trading
- Social Data
- News
- Prediction Markets
- Reddit
- X / Twitter
- Polymarket
- AI Agents
- REST API
- OpenAPI
- llms-txt
- Agent Skills
---
