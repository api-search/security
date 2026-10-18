---
api_specs:
- filename: coincheck-private-api-openapi.yml
  format: yaml
  label: Coincheck Private API
  slug: coincheck-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincheck/refs/heads/main/openapi/coincheck-private-api-openapi.yml
- filename: coincheck-public-api-openapi.yml
  format: yaml
  label: Coincheck Public API
  slug: coincheck-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincheck/refs/heads/main/openapi/coincheck-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coincheck.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: coincheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coincheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coincheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coincheck
provider_slug: coincheck
slug: coincheck-domain-security
source_filename: coincheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coincheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: coincheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coincheck/refs/heads/main/security/coincheck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Japan
---
