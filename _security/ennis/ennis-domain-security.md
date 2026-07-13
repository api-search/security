---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ennis.com
  spf: true
hosts:
- cert_expires: Sep  8 13:10:26 2026 GMT
  host: www.ennis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.ennis.com
  https: false
- host: api.ennis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ennis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ennis Inc, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ennis Inc
provider_slug: ennis
slug: ennis-domain-security
source_filename: ennis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ennis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:10:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ennis.com\n  https: false\n- host: api.ennis.com\n  https: false\ndomains:\n- domain: ennis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ennis/refs/heads/main/security/ennis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Forms
- Printing
- Promotional
---
