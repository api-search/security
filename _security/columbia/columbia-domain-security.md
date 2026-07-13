---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: columbia.edu
  spf: true
hosts:
- cert_expires: Sep  5 23:58:29 2026 GMT
  host: www.columbia.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 09:34:03 2026 GMT
  host: opendataservice.columbia.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: library.columbia.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Columbia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Columbia University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Columbia University
provider_slug: columbia
slug: columbia-domain-security
source_filename: columbia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.columbia.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:58:29 2026 GMT\n  hsts: null\n- host: opendataservice.columbia.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 09:34:03 2026 GMT\n  hsts: null\n- host: library.columbia.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: columbia.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/security/columbia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Library
- Identity
- United States
---
