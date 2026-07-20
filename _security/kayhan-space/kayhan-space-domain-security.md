---
api_specs:
- filename: kayhan-space-satcat-openapi-original.json
  format: json
  label: Satcat Service API
  slug: satcat-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/openapi/kayhan-space-satcat-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kayhan.space
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: satcat.com
  spf: true
hosts:
- cert_expires: Sep 25 18:46:52 2026 GMT
  host: kayhan.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 11 14:30:07 2026 GMT
  host: docs.satcat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.satcat.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kayhan Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kayhan Space, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kayhan Space
provider_slug: kayhan-space
slug: kayhan-space-domain-security
source_filename: kayhan-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kayhan.space\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 18:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.satcat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 14:30:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.satcat.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kayhan.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: satcat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/security/kayhan-space-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Space
- Satellite
- Space Situational Awareness
- Collision Avoidance
- Space Traffic Management
- Aerospace
- Astrodynamics
---
