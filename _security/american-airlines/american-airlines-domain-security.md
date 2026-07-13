---
api_specs:
- filename: american-airlines-runway-developer-api-openapi.yml
  format: yaml
  label: American Airlines Runway Developer API
  slug: runway-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/openapi/american-airlines-runway-developer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aa.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.aa.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: developer.aa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Airlines, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Airlines
provider_slug: american-airlines
slug: american-airlines-domain-security
source_filename: american-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.aa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: aa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-airlines/refs/heads/main/security/american-airlines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Aviation
- Flights
- Travel
- Booking
- Developer Experience
- Fortune 100
---
