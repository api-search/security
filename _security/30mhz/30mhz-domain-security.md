---
api_specs:
- filename: 30mhz-zensie-openapi.json
  format: json
  label: ZENSIE API
  slug: zensie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/openapi/30mhz-zensie-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 30mhz.com
  spf: true
hosts:
- cert_expires: Oct 25 06:21:46 2026 GMT
  host: 30mhz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 05:28:00 2026 GMT
  host: support.30mhz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.30mhz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 30Mhz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 30MHz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 30MHz
provider_slug: 30mhz
slug: 30mhz-domain-security
source_filename: 30mhz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 30mhz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 06:21:46 2026 GMT\n  hsts: false\n- host: support.30mhz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.30mhz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 30mhz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/30mhz/refs/heads/main/security/30mhz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Horticulture
- Agriculture
- AgTech
- Sensors
- Internet of Things
- Greenhouse
- Climate Monitoring
- Time Series Data
- Data Platform
- Netherlands
---
