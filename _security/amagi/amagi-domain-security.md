---
api_specs:
- filename: amagi-mapsor-openapi.yml
  format: yaml
  label: Mapsor API
  slug: mapsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-mapsor-openapi.yml
- filename: amagi-callisto-openapi.yml
  format: yaml
  label: services-amagi-tv API
  slug: services-amagi-tv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/openapi/amagi-callisto-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amagi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Sep 27 09:13:36 2026 GMT
  host: www.amagi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: r5i37dwfp8.execute-api.us-east-1.amazonaws.com
  https: false
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: services.amagi.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amagi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amagi, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amagi
provider_slug: amagi
slug: amagi-domain-security
source_filename: amagi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:13:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: r5i37dwfp8.execute-api.us-east-1.amazonaws.com\n  https: false\n- host: services.amagi.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amagi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amagi/refs/heads/main/security/amagi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Broadcast
- Streaming
- Video
- CTV
- FAST
- Advertising
- Cloud
- Playout
---
