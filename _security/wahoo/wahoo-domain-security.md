---
api_specs:
- filename: wahoo-cloud-api-openapi.yml
  format: yaml
  label: Wahoo Cloud API
  slug: wahoo-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/openapi/wahoo-cloud-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wahoofitness.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wahooligan.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.wahoofitness.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 16:52:18 2026 GMT
  host: cloud-api.wahooligan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.wahooligan.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wahoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wahoo Fitness, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wahoo Fitness
provider_slug: wahoo
slug: wahoo-domain-security
source_filename: wahoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wahoofitness.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud-api.wahooligan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:52:18 2026 GMT\n  hsts: false\n- host: api.wahooligan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: wahoofitness.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wahooligan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wahoo/refs/heads/main/security/wahoo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fitness
- Cycling
- Endurance Training
- Bike Computers
- Smart Trainers
- Indoor Cycling
- Heart Rate
- Power Meters
- GPS
- Wearables
- Hardware
- FIT Files
- Webhooks
- OAuth
---
