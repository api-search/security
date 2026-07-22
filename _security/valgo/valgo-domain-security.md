---
api_specs:
- filename: valgo-humanbaselines-openapi.json
  format: json
  label: Human Crash Baselines API
  slug: human-crash-baselines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/openapi/valgo-humanbaselines-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valgo.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: humanbaselines.com
  spf: false
hosts:
- cert_expires: Oct  3 05:33:24 2026 GMT
  host: valgo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:03:04 2026 GMT
  host: docs.humanbaselines.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:19:06 2026 GMT
  host: humanbaselines.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valgo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Valgo
provider_slug: valgo
slug: valgo-domain-security
source_filename: valgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valgo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:33:24 2026 GMT\n  hsts: false\n- host: docs.humanbaselines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: humanbaselines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:19:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: valgo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: humanbaselines.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valgo/refs/heads/main/security/valgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Risk Management
- Autonomous Vehicles
- Robotics
- Artificial Intelligence
- Safety Validation
- Actuarial
---
