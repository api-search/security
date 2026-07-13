---
api_specs:
- filename: apis
  format: yaml
  label: AYLIEN News API
  slug: news-api
  spec_type: OpenAPI
  url: https://github.com/AYLIEN/apis
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
