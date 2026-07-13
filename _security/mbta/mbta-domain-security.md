---
api_specs:
- filename: mbta-mbta-v3-api-openapi.yml
  format: yaml
  label: MBTA V3 API
  slug: mbta-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-mbta-v3-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mbta.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.mbta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api-v3.mbta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mbta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MBTA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MBTA
provider_slug: mbta
slug: mbta-domain-security
source_filename: mbta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mbta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v3.mbta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mbta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/security/mbta-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Boston
- Massachusetts
- Public Transportation
- Real-Time
- Transit
---
