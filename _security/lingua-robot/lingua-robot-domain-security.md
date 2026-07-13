---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linguarobot.io
  spf: false
hosts:
- cert_expires: Aug 15 14:54:19 2026 GMT
  host: www.linguarobot.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lingua Robot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingua Robot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lingua Robot
provider_slug: lingua-robot
slug: lingua-robot-domain-security
source_filename: lingua-robot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linguarobot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:54:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linguarobot.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingua-robot/refs/heads/main/security/lingua-robot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Dictionaries
- Public APIs
---
