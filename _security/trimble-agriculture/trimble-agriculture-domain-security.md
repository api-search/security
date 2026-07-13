---
api_specs:
- filename: trimble-agriculture-openapi.yml
  format: yaml
  label: Trimble Agriculture Data API
  slug: trimble-agriculture-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-agriculture/refs/heads/main/openapi/trimble-agriculture-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trimble.com
  spf: true
hosts:
- cert_expires: Aug 25 22:53:46 2026 GMT
  host: agriculture.trimble.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: agdeveloper.trimble.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: cloud.api.trimble.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trimble Agriculture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trimble Agriculture, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trimble Agriculture
provider_slug: trimble-agriculture
slug: trimble-agriculture-domain-security
source_filename: trimble-agriculture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agriculture.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: agdeveloper.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: cloud.api.trimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trimble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble-agriculture/refs/heads/main/security/trimble-agriculture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Farming
- IoT
- Precision Agriculture
- Field Management
- Prescriptions
- Telematics
---
