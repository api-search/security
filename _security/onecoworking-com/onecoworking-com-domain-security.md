---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onecoworking.com
  spf: true
hosts:
- cert_expires: Jan  5 04:55:55 2027 GMT
  host: onecoworking.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: One Coworking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Coworking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: One Coworking
provider_slug: onecoworking-com
slug: onecoworking-com-domain-security
source_filename: onecoworking-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onecoworking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 04:55:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: onecoworking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onecoworking-com/security/onecoworking-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Office Matching
- Coworking Spaces
- Private Offices
- Meeting Rooms
- Day Passes
- Flexible Workspace
- Real Estate Services
---
