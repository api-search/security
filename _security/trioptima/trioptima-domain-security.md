---
api_specs:
- filename: trioptima-trireduce-api-openapi.yml
  format: yaml
  label: Trioptima triReduce API
  slug: trireduce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/openapi/trioptima-trireduce-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osttra.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:admin@trioptima.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trireduce.com
  spf: true
hosts:
- cert_expires: Aug 11 22:32:49 2026 GMT
  host: osttra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rates.trireduce.com
  https: false
- host: triresolve.com
  https: false
kind: domain-security
layout: security
method: probed
name: Trioptima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trioptima, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trioptima
provider_slug: trioptima
slug: trioptima-domain-security
source_filename: trioptima-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osttra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 22:32:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rates.trireduce.com\n  https: false\n- host: triresolve.com\n  https: false\ndomains:\n- domain: osttra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: trireduce.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:admin@trioptima.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/security/trioptima-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CME Group
- Derivatives
- Financial Services
- OSTTRA
- Portfolio Compression
- Post-Trade Services
- Reconciliation
- Risk Management
---
