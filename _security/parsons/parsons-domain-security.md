---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: parsons.com
  spf: true
hosts:
- cert_expires: Sep 15 14:40:46 2026 GMT
  host: www.parsons.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.parsons.com
  https: false
- host: api.parsons.com
  https: false
kind: domain-security
layout: security
method: probed
name: Parsons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsons Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Parsons Corporation
provider_slug: parsons
slug: parsons-domain-security
source_filename: parsons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parsons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:40:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.parsons.com\n  https: false\n- host: api.parsons.com\n  https: false\ndomains:\n- domain: parsons.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsons/refs/heads/main/security/parsons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Defense
- Engineering
- Government
---
