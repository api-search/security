---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: csod.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cornerstoneondemand.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: csod.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 12:52:57 2026 GMT
  host: www.cornerstoneondemand.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cornerstone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cornerstone OnDemand, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cornerstone OnDemand
provider_slug: cornerstone
slug: cornerstone-domain-security
source_filename: cornerstone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csod.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.cornerstoneondemand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:52:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: csod.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: cornerstoneondemand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornerstone/refs/heads/main/security/cornerstone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Talent Management
- Learning Management
- Performance Management
- Recruiting
- HR
- Workforce Analytics
- Succession Planning
- Enterprise
---
