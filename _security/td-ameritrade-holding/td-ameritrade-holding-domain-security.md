---
api_specs:
- filename: td-ameritrade-accounts-trading-openapi.yml
  format: yaml
  label: TD Ameritrade Accounts and Trading API
  slug: accounts-and-trading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/openapi/td-ameritrade-accounts-trading-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tdameritrade.com
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: www.tdameritrade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.tdameritrade.com
  https: false
- host: api.tdameritrade.com
  https: false
kind: domain-security
layout: security
method: probed
name: Td Ameritrade Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TD Ameritrade Holding, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TD Ameritrade Holding
provider_slug: td-ameritrade-holding
slug: td-ameritrade-holding-domain-security
source_filename: td-ameritrade-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tdameritrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tdameritrade.com\n  https: false\n- host: api.tdameritrade.com\n  https: false\ndomains:\n- domain: tdameritrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade-holding/refs/heads/main/security/td-ameritrade-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Brokerage
- Trading
- Market Data
- Investment
- Charles Schwab
- Deprecated
- Fortune 1000
---
