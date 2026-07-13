---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hamiltonlane.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.hamiltonlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.hamiltonlane.com
  https: false
- host: api.hamiltonlane.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hamilton Lane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamilton Lane, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hamilton Lane
provider_slug: hamilton-lane
slug: hamilton-lane-domain-security
source_filename: hamilton-lane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hamiltonlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hamiltonlane.com\n  https: false\n- host: api.hamiltonlane.com\n  https: false\ndomains:\n- domain: hamiltonlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hamilton-lane/refs/heads/main/security/hamilton-lane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Private Markets
- Asset Management
- Investment
---
