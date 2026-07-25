---
api_specs:
- filename: aylien-absa-api-openapi.yml
  format: yaml
  label: AYLIEN Absa API
  slug: aylien-absa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-absa-api-openapi.yml
- filename: aylien-autocomplete-api-openapi.yml
  format: yaml
  label: AYLIEN autocomplete API
  slug: aylien-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-autocomplete-api-openapi.yml
- filename: aylien-classify-api-openapi.yml
  format: yaml
  label: AYLIEN Classify API
  slug: aylien-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-classify-api-openapi.yml
- filename: aylien-cluster-api-openapi.yml
  format: yaml
  label: AYLIEN cluster API
  slug: aylien-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-cluster-api-openapi.yml
- filename: aylien-concepts-api-openapi.yml
  format: yaml
  label: AYLIEN Concepts API
  slug: aylien-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-concepts-api-openapi.yml
- filename: aylien-elsa-api-openapi.yml
  format: yaml
  label: AYLIEN Elsa API
  slug: aylien-elsa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-elsa-api-openapi.yml
- filename: aylien-entities-api-openapi.yml
  format: yaml
  label: AYLIEN Entities API
  slug: aylien-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-entities-api-openapi.yml
- filename: aylien-extract-api-openapi.yml
  format: yaml
  label: AYLIEN Extract API
  slug: aylien-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-extract-api-openapi.yml
- filename: aylien-hashtags-api-openapi.yml
  format: yaml
  label: AYLIEN Hashtags API
  slug: aylien-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-hashtags-api-openapi.yml
- filename: aylien-histogram-api-openapi.yml
  format: yaml
  label: AYLIEN histogram API
  slug: aylien-histogram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-histogram-api-openapi.yml
- filename: aylien-language-api-openapi.yml
  format: yaml
  label: AYLIEN Language API
  slug: aylien-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-language-api-openapi.yml
- filename: aylien-related-story-api-openapi.yml
  format: yaml
  label: AYLIEN related_story API
  slug: aylien-related-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-related-story-api-openapi.yml
- filename: aylien-sentiment-api-openapi.yml
  format: yaml
  label: AYLIEN Sentiment API
  slug: aylien-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-sentiment-api-openapi.yml
- filename: aylien-story-api-openapi.yml
  format: yaml
  label: AYLIEN story API
  slug: aylien-story-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-story-api-openapi.yml
- filename: aylien-summarize-api-openapi.yml
  format: yaml
  label: AYLIEN Summarize API
  slug: aylien-summarize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-summarize-api-openapi.yml
- filename: aylien-time-series-api-openapi.yml
  format: yaml
  label: AYLIEN time_series API
  slug: aylien-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-time-series-api-openapi.yml
- filename: aylien-trends-api-openapi.yml
  format: yaml
  label: AYLIEN trends API
  slug: aylien-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/openapi/aylien-trends-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aylien.com
  spf: true
hosts:
- host: aylien.com
  https: false
- host: api.aylien.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aylien Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AYLIEN, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AYLIEN
provider_slug: aylien
slug: aylien-domain-security
source_filename: aylien-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aylien.com\n  https: false\n- host: api.aylien.com\n  https: false\ndomains:\n- domain: aylien.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aylien/refs/heads/main/security/aylien-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- News Intelligence
- Text Analysis
- NLP
- Sentiment Analysis
- Entity Recognition
- Natural Language Processing
- News API
- Article Extraction
- Summarization
- Concept Detection
---
