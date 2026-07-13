---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Refinitiv Data Platform APIs
  slug: refinitiv-data-platform-apis
  spec_type: OpenAPI
  url: https://api.refinitiv.com/streaming-pricing/docs/swagger.yaml
- filename: refinitiv-eikon-asyncapi.yml
  format: yaml
  label: LSEG WebSocket API
  slug: lseg-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/asyncapi/refinitiv-eikon-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lseg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: refinitiv.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developers.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: www.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.refinitiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refinitiv Eikon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refinitiv Eikon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Refinitiv Eikon
provider_slug: refinitiv-eikon
slug: refinitiv-eikon-domain-security
source_filename: refinitiv-eikon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.refinitiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lseg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: refinitiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/security/refinitiv-eikon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Financial Data
- Financial News
- Market Data
- Real-Time Data
- Trading
---
