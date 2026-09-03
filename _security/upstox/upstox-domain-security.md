---
api_specs:
- filename: upstox-developer-api-openapi.yml
  format: yaml
  label: Upstox Developer API
  slug: upstox-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/openapi/upstox-developer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upstox.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: upstox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 20:00:28 2026 GMT
  host: api.upstox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 14:33:25 2026 GMT
  host: mcp.upstox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upstox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upstox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upstox
provider_slug: upstox
slug: upstox-domain-security
source_filename: upstox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upstox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upstox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 20:00:28 2026 GMT\n  hsts: null\n- host: mcp.upstox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 14:33:25 2026 GMT\n  hsts: null\ndomains:\n- domain: upstox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/security/upstox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Stock Trading
- Brokerage
- Market Data
- Investing
- Capital Markets
- Mutual Funds
- Algorithmic Trading
- India
---
