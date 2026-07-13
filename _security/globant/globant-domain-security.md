---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globant.com
  spf: true
hosts:
- cert_expires: Sep 24 05:28:27 2026 GMT
  host: www.globant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.globant.com
  https: false
- cert_expires: Oct 14 15:41:53 2026 GMT
  host: api.globant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Globant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globant, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Globant
provider_slug: globant
slug: globant-domain-security
source_filename: globant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:28:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.globant.com\n  https: false\n- host: api.globant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:41:53 2026 GMT\n  hsts: null\ndomains:\n- domain: globant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globant/refs/heads/main/security/globant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software
- Digital Transformation
- AI
---
