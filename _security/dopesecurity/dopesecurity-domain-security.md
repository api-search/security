---
api_specs:
- filename: dopesecurity-flightdeck-openapi.yml
  format: yaml
  label: Flightdeck API
  slug: flightdeck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/openapi/dopesecurity-flightdeck-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dope.security
  spf: true
hosts:
- cert_expires: Oct 16 04:03:14 2026 GMT
  host: dope.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 22:59:30 2026 GMT
  host: inflight.dope.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.flightdeck.dope.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dopesecurity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dope.security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dope.security
provider_slug: dopesecurity
slug: dopesecurity-domain-security
source_filename: dopesecurity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dope.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 04:03:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: inflight.dope.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:59:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flightdeck.dope.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dope.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopesecurity/refs/heads/main/security/dopesecurity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Security
- Cybersecurity
- Secure Web Gateway
- SASE
- SSE
- Data Loss Prevention
- CASB
- Endpoint Security
- API
---
