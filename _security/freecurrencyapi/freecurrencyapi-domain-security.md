---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Free Currency API
  slug: freecurrencyapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freecurrencyapi/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freecurrencyapi.com
  spf: true
hosts:
- cert_expires: Aug 31 04:18:49 2026 GMT
  host: freecurrencyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:18:49 2026 GMT
  host: api.freecurrencyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freecurrencyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Currency API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Free Currency API
provider_slug: freecurrencyapi
slug: freecurrencyapi-domain-security
source_filename: freecurrencyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freecurrencyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:18:49 2026 GMT\n  hsts: false\n- host: api.freecurrencyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:18:49 2026 GMT\n  hsts: null\ndomains:\n- domain: freecurrencyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freecurrencyapi/refs/heads/main/security/freecurrencyapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency
- Exchange Rates
- Finance
- Historical Data
- Free
---
