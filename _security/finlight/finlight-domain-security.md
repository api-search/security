---
api_specs:
- filename: openapi.json
  format: json
  label: Finlight Financial News API
  slug: finlight-financial-news-api
  spec_type: OpenAPI
  url: https://docs.finlight.me/v2/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finlight.me
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: finlight.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.finlight.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finlight, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Finlight
provider_slug: finlight
slug: finlight-domain-security
source_filename: finlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finlight.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: api.finlight.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: finlight.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finlight/refs/heads/main/security/finlight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial News
- Sentiment Analysis
- Market Data
- Equities
- Currencies
- Commodities
- Real-Time
- Webhooks
- WebSocket
---
