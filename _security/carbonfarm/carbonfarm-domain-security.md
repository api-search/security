---
api_specs:
- filename: carbonfarm-cms-openapi.json
  format: json
  label: CarbonFarm CMS Content API
  slug: carbonfarm-cms-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/openapi/carbonfarm-cms-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: carbonfarm.tech
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: carbonfarm.app
  spf: false
hosts:
- cert_expires: Sep 30 03:11:37 2026 GMT
  host: www.carbonfarm.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 05:55:05 2026 GMT
  host: cms.int.carbonfarm.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbonfarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarbonFarm, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CarbonFarm
provider_slug: carbonfarm
slug: carbonfarm-domain-security
source_filename: carbonfarm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carbonfarm.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:11:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cms.int.carbonfarm.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 05:55:05 2026 GMT\n  hsts: null\ndomains:\n- domain: carbonfarm.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: carbonfarm.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonfarm/refs/heads/main/security/carbonfarm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate Tech
- Carbon Credits
- Agriculture
- MRV
- Satellite Imagery
- Remote Sensing
- Machine-Learning
- Sustainability
- Content Management
---
