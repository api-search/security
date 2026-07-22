---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 9mothers.com
  spf: true
hosts:
- cert_expires: Aug 25 20:48:33 2026 GMT
  host: 9mothers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 9 Mothers Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9 Mothers Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 9 Mothers Corporation
provider_slug: 9-mothers-corporation
slug: 9-mothers-corporation-domain-security
source_filename: 9-mothers-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 9mothers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:48:33 2026 GMT\n  hsts: false\ndomains:\n- domain: 9mothers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9-mothers-corporation/refs/heads/main/security/9-mothers-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defense
- Counter-Drone
- Autonomous Systems
- Robotics
- Hardware
- Security
- Y Combinator
---
