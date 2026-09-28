---
api_specs:
- filename: rtcstats-rtcstats-api-api-openapi.yml
  format: yaml
  label: rtcStats API
  slug: rtcstats-rtcstats-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtcstats/refs/heads/main/openapi/rtcstats-rtcstats-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rtcstats.com
  spf: true
hosts:
- cert_expires: Dec  6 14:53:03 2026 GMT
  host: www.rtcstats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 04:48:28 2026 GMT
  host: rtcstats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 15:30:38 2026 GMT
  host: api.rtcstats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rtcstats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rtcStats, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: rtcStats
provider_slug: rtcstats
slug: rtcstats-domain-security
source_filename: rtcstats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtcstats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 14:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rtcstats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 04:48:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rtcstats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 15:30:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rtcstats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtcstats/refs/heads/main/security/rtcstats-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WebRTC
- Observability
- Monitoring
- Debugging
- Real-Time Communication
- Video
- Voice
- Artificial Intelligence
- MCP
- Developer Tools
---
