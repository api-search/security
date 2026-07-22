---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scodix.com
  spf: true
hosts:
- cert_expires: Oct  7 11:50:54 2026 GMT
  host: scodix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scodix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scodix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scodix
provider_slug: scodix
slug: scodix-domain-security
source_filename: scodix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scodix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:50:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scodix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scodix/refs/heads/main/security/scodix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Printing
- Digital Printing
- Embellishment
- Packaging
- Web-to-Print
- Manufacturing
- Print Technology
---
