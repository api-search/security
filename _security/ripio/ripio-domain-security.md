---
api_specs:
- filename: ripio-trade-openapi.yml
  format: yaml
  label: Ripio Trade API v4
  slug: ripio-trade-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/openapi/ripio-trade-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ripio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ripiotrade.co
  spf: true
hosts:
- cert_expires: Oct 12 03:44:01 2026 GMT
  host: www.ripio.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 05:01:43 2026 GMT
  host: api.ripiotrade.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ripio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ripio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ripio
provider_slug: ripio
slug: ripio-domain-security
source_filename: ripio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ripio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:44:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.ripiotrade.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:01:43 2026 GMT\n  hsts: null\ndomains:\n- domain: ripio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ripiotrade.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripio/refs/heads/main/security/ripio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Latin America
- Bitcoin
- Stablecoins
- API
---
