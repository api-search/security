---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curaum.com
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: curaum.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curaum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curaum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Curaum
provider_slug: curaum
slug: curaum-domain-security
source_filename: curaum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curaum.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: curaum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curaum/refs/heads/main/security/curaum-domain-security.yml
summary_line: TLSv1.2
tags:
- Healthcare
- IoMT
- DentalTech
- SleepHealth
- Korean
---
