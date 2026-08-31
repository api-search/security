---
api_key_in:
- header
api_specs:
- filename: bitvore-alert-api-api-openapi.yml
  format: yaml
  label: Bitvore Alert API API
  slug: bitvore-alert-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-alert-api-api-openapi.yml
- filename: bitvore-bond-api-openapi.yml
  format: yaml
  label: Bitvore Bond API
  slug: bitvore-bond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-bond-api-openapi.yml
- filename: bitvore-corporate-news-api-openapi.yml
  format: yaml
  label: Bitvore Corporate News API
  slug: bitvore-corporate-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-corporate-news-api-openapi.yml
- filename: bitvore-datasets-api-api-openapi.yml
  format: yaml
  label: Bitvore Datasets API API
  slug: bitvore-datasets-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-datasets-api-api-openapi.yml
- filename: bitvore-economic-news-api-openapi.yml
  format: yaml
  label: Bitvore Economic News API
  slug: bitvore-economic-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-economic-news-api-openapi.yml
- filename: bitvore-entity-api-openapi.yml
  format: yaml
  label: Bitvore Entity API
  slug: bitvore-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-entity-api-openapi.yml
- filename: bitvore-filings-api-api-openapi.yml
  format: yaml
  label: Bitvore Filings API API
  slug: bitvore-filings-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-filings-api-api-openapi.yml
- filename: bitvore-financial-filings-api-openapi.yml
  format: yaml
  label: Bitvore Financial Filings API
  slug: bitvore-financial-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-financial-filings-api-openapi.yml
- filename: bitvore-identification-api-openapi.yml
  format: yaml
  label: Bitvore Identification API
  slug: bitvore-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-identification-api-openapi.yml
- filename: bitvore-intel-api-openapi.yml
  format: yaml
  label: Bitvore Intel API
  slug: bitvore-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-intel-api-openapi.yml
- filename: bitvore-muni-api-api-openapi.yml
  format: yaml
  label: Bitvore Muni API API
  slug: bitvore-muni-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-muni-api-api-openapi.yml
- filename: bitvore-muni-news-api-openapi.yml
  format: yaml
  label: Bitvore Muni News API
  slug: bitvore-muni-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-muni-news-api-openapi.yml
- filename: bitvore-news-api-api-openapi.yml
  format: yaml
  label: Bitvore News API API
  slug: bitvore-news-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-news-api-api-openapi.yml
- filename: bitvore-oauth2-api-openapi.yml
  format: yaml
  label: Bitvore O Auth2 API
  slug: bitvore-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-oauth2-api-openapi.yml
- filename: bitvore-organizations-api-api-openapi.yml
  format: yaml
  label: Bitvore Organizations API API
  slug: bitvore-organizations-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-organizations-api-api-openapi.yml
- filename: bitvore-portfolio-api-openapi.yml
  format: yaml
  label: Bitvore Portfolio API
  slug: bitvore-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-portfolio-api-openapi.yml
- filename: bitvore-portfolios-api-api-openapi.yml
  format: yaml
  label: Bitvore Portfolios API API
  slug: bitvore-portfolios-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-portfolios-api-api-openapi.yml
- filename: bitvore-sentiment-scores-api-api-openapi.yml
  format: yaml
  label: Bitvore Sentiment Scores API API
  slug: bitvore-sentiment-scores-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-sentiment-scores-api-api-openapi.yml
- filename: bitvore-sentiment-scores-api-openapi.yml
  format: yaml
  label: Bitvore Sentiment Scores API
  slug: bitvore-sentiment-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/openapi/bitvore-sentiment-scores-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bitvore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bitvore secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bitvore
provider_slug: bitvore
scheme_count: 3
schemes:
- in: header
  name: API key
  parameter: X-BV-APIKEY
  sources:
  - openapi/_original/bitvore-corporate-openapi.yml
  - openapi/_original/bitvore-legacy-openapi.yml
  - openapi/_original/bitvore-muni-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.bitvore.com/oauth/accesstoken
  name: OAuth
  sources:
  - openapi/_original/bitvore-corporate-openapi.yml
  - openapi/_original/bitvore-legacy-openapi.yml
  - openapi/_original/bitvore-muni-openapi.yml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/_original/bitvore-custom-api-it-openapi.yml
  - openapi/_original/bitvore-custom-api-l-openapi.yml
  - openapi/_original/bitvore-legacy-openapi.yml
  type: http
slug: bitvore-authentication
source_filename: bitvore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: derived\nsource: openapi/_original/bitvore-corporate-openapi.yml, openapi/_original/bitvore-custom-api-it-openapi.yml, openapi/_original/bitvore-custom-api-l-openapi.yml,\n  openapi/_original/bitvore-legacy-openapi.yml, openapi/_original/bitvore-muni-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: API key\n  type: apiKey\n  in: header\n  parameter: X-BV-APIKEY\n  sources:\n  - openapi/_original/bitvore-corporate-openapi.yml\n  - openapi/_original/bitvore-legacy-openapi.yml\n  - openapi/_original/bitvore-muni-openapi.yml\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.bitvore.com/oauth/accesstoken\n    scopes: 1\n  sources:\n  - openapi/_original/bitvore-corporate-openapi.yml\n  - openapi/_original/bitvore-legacy-openapi.yml\n  - openapi/_original/bitvore-muni-openapi.yml\n- name: BasicAuth\n\
  \  type: http\n  scheme: basic\n  sources:\n  - openapi/_original/bitvore-custom-api-it-openapi.yml\n  - openapi/_original/bitvore-custom-api-l-openapi.yml\n  - openapi/_original/bitvore-legacy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitvore/refs/heads/main/authentication/bitvore-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Financial Data
- Market Intelligence
- alternative-data
- news-api
- NLP
- ESG
- municipal-bonds
- credit-risk
- company-data
- sentiment-analysis
- unstructured-data
- fixed-income
---
