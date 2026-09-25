---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agerpoint.com
  spf: true
hosts:
- cert_expires: Oct 25 22:16:37 2026 GMT
  host: www.agerpoint.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: cloudapi.agerpoint.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agerpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agerpoint, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agerpoint
provider_slug: agerpoint
slug: agerpoint-domain-security
source_filename: agerpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agerpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 22:16:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: cloudapi.agerpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agerpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agerpoint/refs/heads/main/security/agerpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Geospatial
- Remote Sensing
- Digital Twin
- LiDAR
- Point Cloud
- Carbon Measurement
- Forestry
- Machine Learning
- Spatial Analytics
- Company
---
