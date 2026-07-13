---
api_specs:
- filename: lseg-world-check-one-openapi-original.yml
  format: yaml
  label: LSEG World-Check One API
  slug: lseg-world-check-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/lseg-world-check-one-openapi-original.yml
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
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: www.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api-worldcheck.refinitiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: London Stock Exchange Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for London Stock Exchange Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: London Stock Exchange Group
provider_slug: london-stock-exchange-group
slug: london-stock-exchange-group-domain-security
source_filename: london-stock-exchange-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-worldcheck.refinitiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lseg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: refinitiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/security/london-stock-exchange-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Stock Exchange
- Market Data
- KYC
- Compliance
---
