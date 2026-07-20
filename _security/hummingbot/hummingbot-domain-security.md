---
api_specs:
- filename: hummingbot-gateway-openapi-original.json
  format: json
  label: Hummingbot Gateway
  slug: hummingbot-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingbot/refs/heads/main/openapi/hummingbot-gateway-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hummingbot.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hummingbot.org
  spf: true
hosts:
- cert_expires: Sep 21 08:21:41 2026 GMT
  host: hummingbot.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:40:48 2026 GMT
  host: hummingbot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hummingbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hummingbot, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hummingbot
provider_slug: hummingbot
slug: hummingbot-domain-security
source_filename: hummingbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hummingbot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:21:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hummingbot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:40:48 2026 GMT\n  hsts: false\ndomains:\n- domain: hummingbot.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hummingbot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hummingbot/refs/heads/main/security/hummingbot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Trading
- Blockchain
- DeFi
- DEX
- Open Source
- Market Making
- Algorithmic Trading
- Bots
---
