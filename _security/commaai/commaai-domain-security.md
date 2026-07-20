---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comma.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: commadotai.com
  spf: false
hosts:
- cert_expires: Aug 27 11:42:56 2026 GMT
  host: comma.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 05:27:07 2026 GMT
  host: api.comma.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 05:43:28 2026 GMT
  host: api.commadotai.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comma.ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Comma.ai
provider_slug: commaai
slug: commaai-domain-security
source_filename: commaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.comma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:27:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.commadotai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:43:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: comma.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: commadotai.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commaai/refs/heads/main/security/commaai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Self-Driving
- Robotics
- Artificial Intelligence
- Machine Learning
- Open Source
- Connected Vehicles
- Telematics
- Developer API
---
