---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doodle.com
  spf: true
hosts:
- cert_expires: Sep  1 04:00:01 2026 GMT
  host: doodle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:00:01 2026 GMT
  host: help.doodle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doodle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doodle, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Doodle
provider_slug: doodle
slug: doodle-domain-security
source_filename: doodle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doodle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.doodle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doodle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doodle/refs/heads/main/security/doodle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Scheduling
- Meetings
- Calendar
- Group Polls
- Booking Pages
- Time Management
- Productivity
---
