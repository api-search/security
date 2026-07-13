---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arconic.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kawneer.com
  spf: true
hosts:
- cert_expires: Sep 14 12:02:06 2026 GMT
  host: www.arconic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 12:30:10 2026 GMT
  host: crms.arconic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.kawneer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arconic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arconic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arconic
provider_slug: arconic
slug: arconic-domain-security
source_filename: arconic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arconic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:02:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: crms.arconic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:30:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.kawneer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arconic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kawneer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arconic/refs/heads/main/security/arconic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aluminum
- Manufacturing
- Extrusions
- Rolled Products
- Building Products
- Architectural Systems
- Aerospace
- Automotive
- Packaging
---
