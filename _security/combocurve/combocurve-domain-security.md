---
api_specs:
- filename: combocurve-openapi.yml
  format: yaml
  label: ComboCurve REST API
  slug: combocurve-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/combocurve/refs/heads/main/openapi/combocurve-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: combocurve.com
  spf: true
hosts:
- cert_expires: Sep 23 21:43:31 2026 GMT
  host: combocurve.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 19:30:03 2026 GMT
  host: api.combocurve.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Combocurve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComboCurve, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ComboCurve
provider_slug: combocurve
slug: combocurve-domain-security
source_filename: combocurve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: combocurve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.combocurve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:30:03 2026 GMT\n  hsts: null\ndomains:\n- domain: combocurve.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/combocurve/refs/heads/main/security/combocurve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Oil and Gas
- Energy
- Forecasting
- Reserves
- Economics
- Upstream
- Petroleum Engineering
---
