---
api_specs:
- filename: openapi.json
  format: json
  label: Adanos Market Sentiment API
  slug: adanos-market-sentiment-api
  spec_type: OpenAPI
  url: https://api.adanos.org/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adanos.org
  spf: true
hosts:
- cert_expires: Nov 23 10:15:45 2026 GMT
  host: api.adanos.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adanos Market Sentiment Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adanos Market Sentiment API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adanos Market Sentiment API
provider_slug: adanos-market-sentiment-api
slug: adanos-market-sentiment-api-domain-security
source_filename: adanos-market-sentiment-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.adanos.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 10:15:45 2026 GMT\n  hsts: null\ndomains:\n- domain: adanos.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adanos-market-sentiment-api/refs/heads/main/security/adanos-market-sentiment-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
