---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unison-lang.org
  spf: false
hosts:
- cert_expires: Sep 21 03:43:48 2026 GMT
  host: www.unison-lang.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 17:33:50 2026 GMT
  host: share.unison-lang.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:06 2026 GMT
  host: api.unison-lang.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unison Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unison Computing, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Unison Computing
provider_slug: unison-computing
slug: unison-computing-domain-security
source_filename: unison-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unison-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: share.unison-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 17:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unison-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:06 2026 GMT\n  hsts: null\ndomains:\n- domain: unison-lang.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unison-computing/refs/heads/main/security/unison-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Programming Languages
- Cloud Computing
- Developer Tools
- Functional Programming
- Distributed Systems
- Platform as a Service
---
