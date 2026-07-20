---
api_specs:
- filename: kumospace-api-openapi.json
  format: json
  label: Kumospace API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kumospace/refs/heads/main/openapi/kumospace-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kumospace.com
  spf: true
hosts:
- cert_expires: Aug 26 09:39:26 2026 GMT
  host: www.kumospace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:10:39 2026 GMT
  host: api.kumospace.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kumospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kumospace, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kumospace
provider_slug: kumospace
slug: kumospace-domain-security
source_filename: kumospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kumospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:39:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kumospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:10:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kumospace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kumospace/refs/heads/main/security/kumospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtual Office
- Remote Work
- Collaboration
- Video Conferencing
- Communications
- Real Time
- Productivity
- Meetings
- Spatial Audio
---
