---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cropx.com
  spf: true
hosts:
- cert_expires: Oct  9 15:41:23 2026 GMT
  host: cropx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 16:37:17 2026 GMT
  host: app.cropx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cropx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CropX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CropX
provider_slug: cropx
slug: cropx-domain-security
source_filename: cropx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.cropx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: cropx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cropx/refs/heads/main/security/cropx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- AgTech
- IoT
- Soil Sensors
- Irrigation
- Farm Management
---
