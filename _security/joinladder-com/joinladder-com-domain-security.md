---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinladder.com
  spf: true
hosts:
- cert_expires: Jan 21 21:31:25 2027 GMT
  host: www.joinladder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joinladder Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ladder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ladder
provider_slug: joinladder-com
slug: joinladder-com-domain-security
source_filename: joinladder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinladder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 21:31:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinladder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/joinladder-com/security/joinladder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fitness
- Health
- Personalization
- Coaching
---
