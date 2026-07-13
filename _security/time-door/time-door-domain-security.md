---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: timedoor.io
  spf: false
hosts:
- cert_expires: Sep 17 17:20:32 2026 GMT
  host: timedoor.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Time Door Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Time Door, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Time Door
provider_slug: time-door
slug: time-door-domain-security
source_filename: time-door-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timedoor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:20:32 2026 GMT\n  hsts: false\ndomains:\n- domain: timedoor.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/time-door/refs/heads/main/security/time-door-domain-security.yml
summary_line: TLSv1.3
tags:
- Machine Learning
- Public APIs
---
