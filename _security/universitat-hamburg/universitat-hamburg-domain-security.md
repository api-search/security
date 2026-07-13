---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uni-hamburg.de
  spf: true
hosts:
- cert_expires: Sep  5 02:56:55 2026 GMT
  host: www.uni-hamburg.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 07:57:40 2026 GMT
  host: www.sub.uni-hamburg.de
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:23:43 2026 GMT
  host: ediss.sub.uni-hamburg.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universitat Hamburg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universität Hamburg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Universität Hamburg
provider_slug: universitat-hamburg
slug: universitat-hamburg-domain-security
source_filename: universitat-hamburg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uni-hamburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 02:56:55 2026 GMT\n  hsts: false\n- host: www.sub.uni-hamburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:57:40 2026 GMT\n  hsts: null\n- host: ediss.sub.uni-hamburg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uni-hamburg.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universitat-hamburg/refs/heads/main/security/universitat-hamburg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Germany
- Open Access
- Library
- Metadata
- OAI-PMH
---
