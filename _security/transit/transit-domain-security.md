---
api_specs:
- filename: transit-openapi.yml
  format: yaml
  label: Transit API
  slug: transit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transitapp.com
  spf: true
hosts:
- cert_expires: Aug 18 01:29:20 2026 GMT
  host: transitapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 11:34:48 2026 GMT
  host: api-doc.transitapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transit
provider_slug: transit
slug: transit-domain-security
source_filename: transit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:29:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-doc.transitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:34:48 2026 GMT\n  hsts: false\ndomains:\n- domain: transitapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/security/transit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Public Transit
- Real-Time
- Trip Planning
- Multimodal
- GTFS
- GOFS
- Mobility
- Shared Mobility
---
