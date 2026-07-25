---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: in-toto.io
  spf: false
hosts:
- cert_expires: Sep 11 02:23:22 2026 GMT
  host: in-toto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: In Toto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for In-Toto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: In-Toto
provider_slug: in-toto
slug: in-toto-domain-security
source_filename: in-toto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: in-toto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:23:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: in-toto.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/in-toto/refs/heads/main/security/in-toto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Graduated
- Security
- Software Integrity
- Supply Chain Security
- Verification
---
