---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Trading 212 Public API
  slug: trading-212-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trading212/refs/heads/main/openapi/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trading212.com
  spf: true
hosts:
- cert_expires: Aug 27 07:21:53 2026 GMT
  host: docs.trading212.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 10:45:18 2026 GMT
  host: live.trading212.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 10:45:18 2026 GMT
  host: demo.trading212.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trading212 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trading 212, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trading 212
provider_slug: trading212
slug: trading212-domain-security
source_filename: trading212-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.trading212.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 07:21:53 2026 GMT\n  hsts: false\n- host: live.trading212.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 10:45:18 2026 GMT\n  hsts: null\n- host: demo.trading212.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 10:45:18 2026 GMT\n  hsts: null\ndomains:\n- domain: trading212.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trading212/refs/heads/main/security/trading212-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Investing
- Finance
- Trading
- Stocks
- Portfolio
- Commission-Free
- ISA
---
