---
api_specs:
- filename: ally-invest-openapi.yml
  format: yaml
  label: Ally Invest Accounts API
  slug: ally-invest-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ally-invest/refs/heads/main/openapi/ally-invest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ally.com
  spf: true
hosts:
- cert_expires: Sep  2 04:00:00 2026 GMT
  host: www.ally.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.ally.com
  https: false
- host: stream.ally.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ally Invest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ally Invest, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ally Invest
provider_slug: ally-invest
slug: ally-invest-domain-security
source_filename: ally-invest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ally.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:00:00 2026 GMT\n  hsts: null\n- host: api.ally.com\n  https: false\n- host: stream.ally.com\n  https: false\ndomains:\n- domain: ally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ally-invest/refs/heads/main/security/ally-invest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Brokerage
- Investing
- Trading
- Finance
- Stocks
- Options
- Market Data
- Self-Directed
---
