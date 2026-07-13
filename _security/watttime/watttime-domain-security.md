---
api_specs:
- filename: watttime-openapi.yml
  format: yaml
  label: WattTime API
  slug: watttime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watttime/refs/heads/main/openapi/watttime-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: watttime.org
  spf: true
hosts:
- cert_expires: Oct  7 02:00:55 2026 GMT
  host: watttime.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: docs.watttime.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 13:14:00 2026 GMT
  host: api.watttime.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Watttime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WattTime, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WattTime
provider_slug: watttime
slug: watttime-domain-security
source_filename: watttime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: watttime.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:00:55 2026 GMT\n  hsts: false\n- host: docs.watttime.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\n- host: api.watttime.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 13:14:00 2026 GMT\n  hsts: false\ndomains:\n- domain: watttime.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watttime/refs/heads/main/security/watttime-domain-security.yml
summary_line: TLSv1.3
tags:
- Emissions
- Climate
- Carbon
- Energy
- Electricity Grid
- Sustainability
- Clean Energy
---
