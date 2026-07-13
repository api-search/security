---
api_specs:
- filename: rainbow-ai-nowcast-openapi.yml
  format: yaml
  label: Rainbow.AI Nowcast API
  slug: rainbow-ai-nowcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/openapi/rainbow-ai-nowcast-openapi.yml
- filename: rainbow-ai-tiles-openapi.yml
  format: yaml
  label: Rainbow.AI Tiles API
  slug: rainbow-ai-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/openapi/rainbow-ai-tiles-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rainbow.ai
  spf: true
hosts:
- cert_expires: Aug 23 22:11:55 2026 GMT
  host: www.rainbow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:59:52 2026 GMT
  host: doc.rainbow.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:15:26 2026 GMT
  host: api.rainbow.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainbow Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainbow.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rainbow.AI
provider_slug: rainbow-ai
slug: rainbow-ai-domain-security
source_filename: rainbow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rainbow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:11:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.rainbow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:59:52 2026 GMT\n  hsts: false\n- host: api.rainbow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:15:26 2026 GMT\n  hsts: null\ndomains:\n- domain: rainbow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbow-ai/refs/heads/main/security/rainbow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Precipitation
- Forecasting
- Nowcast
- Radar
- Tiles
- Geospatial
---
